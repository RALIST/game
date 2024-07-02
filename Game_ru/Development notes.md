### Directory Structure
```
wasteland-chronicles/
├── cmd/
│   └── server/
│       └── main.go
├── internal/
│   ├── entities/
│   │   ├── character.go
│   │   ├── item.go
│   │   ├── settlement.go
│   │   └── event.go
│   ├── usecases/
│   │   ├── character_usecase.go
│   │   ├── item_usecase.go
│   │   ├── settlement_usecase.go
│   │   └── event_usecase.go
│   ├── interfaces/
│   │   ├── controllers/
│   │   │   ├── character_controller.go
│   │   │   ├── item_controller.go
│   │   │   ├── settlement_controller.go
│   │   │   └── event_controller.go
│   │   ├── repositories/
│   │   │   ├── character_repository.go
│   │   │   ├── item_repository.go
│   │   │   ├── settlement_repository.go
│   │   │   └── event_repository.go
│   │   └── websocket/
│   │       └── websocket_adapter.go
│   ├── frameworks/
│   │   ├── database/
│   │   │   ├── postgres.go
│   │   │   └── redis.go
│   │   └── logging/
│   │       └── logger.go
├── pkg/
│   ├── config/
│   │   └── config.go
│   ├── middleware/
│   │   └── auth.go
│   └── utils/
│       └── validation.go
└── go.mod
```

### Detailed File Contents

#### `cmd/server/main.go`
This is the entry point of the application.
```go
package main

import (
    "log"
    "net/http"
    "wasteland-chronicles/internal/interfaces/websocket"
    "wasteland-chronicles/pkg/config"
)

func main() {
    cfg := config.LoadConfig()

    http.HandleFunc("/ws", func(w http.ResponseWriter, r *http.Request) {
        wsAdapter, err := websocket.NewWebSocketAdapter(w, r)
        if err != nil {
            log.Println("Error creating WebSocket connection:", err)
            return
        }
        defer wsAdapter.Close()
        for {
            message, err := wsAdapter.ReceiveMessage()
            if err != nil {
                log.Println("Error receiving message:", err)
                break
            }
            log.Println("Received message:", string(message))
            // Handle the message and send a response
            response := []byte("Message received")
            if err := wsAdapter.SendMessage(response); err != nil {
                log.Println("Error sending message:", err)
                break
            }
        }
    })

    log.Println("Server started on :", cfg.ServerPort)
    log.Fatal(http.ListenAndServe(":"+cfg.ServerPort, nil))
}
```

#### `internal/entities/character.go`
Defines the character entity.
```go
package entities

type Attributes struct {
    Strength    int
    Perception  int
    Endurance   int
    Charisma    int
    Intelligence int
    Agility     int
    Luck        int
}

type Stats struct {
    HP               int
    AP               int
    CarryingCapacity int
    HealingRate      int
    CriticalChance   int
    RadiationResistance int
    Reputation       int
    Karma            int
    Fatigue          int
    Level            int
    XP               int
}

type Character struct {
    ID         string
    Name       string
    Attributes Attributes
    Stats      Stats
}

func (c *Character) CalculateDamage() int {
    return c.Attributes.Strength * 2 // Example logic
}

func (c *Character) CalculateCarryingCapacity() int {
    return c.Attributes.Strength * 10 // Example logic
}

func (c *Character) CalculateSkillCheck(skill string) bool {
    switch skill {
    case "strength":
        return c.Attributes.Strength > 10
    case "perception":
        return c.Attributes.Perception > 10
    default:
        return false
    }
}
```

#### `internal/usecases/character_usecase.go`
Defines the use cases for character operations.
```go
package usecases

import "wasteland-chronicles/internal/entities"

type CharacterRepository interface {
    Save(character *entities.Character) error
    Update(character *entities.Character) error
    Delete(id string) error
    FindByID(id string) (*entities.Character, error)
}

type CharacterUseCase struct {
    repo CharacterRepository
}

func NewCharacterUseCase(repo CharacterRepository) *CharacterUseCase {
    return &CharacterUseCase{repo: repo}
}

func (uc *CharacterUseCase) CreateCharacter(character *entities.Character) error {
    return uc.repo.Save(character)
}

func (uc *CharacterUseCase) UpdateCharacter(character *entities.Character) error {
    return uc.repo.Update(character)
}

func (uc *CharacterUseCase) DeleteCharacter(id string) error {
    return uc.repo.Delete(id)
}

func (uc *CharacterUseCase) GetCharacter(id string) (*entities.Character, error) {
    return uc.repo.FindByID(id)
}
```

#### `internal/interfaces/controllers/character_controller.go`
Defines the controller for handling character-related HTTP requests.
```go
package controllers

import (
    "encoding/json"
    "net/http"
    "wasteland-chronicles/internal/entities"
    "wasteland-chronicles/internal/usecases"
)

type CharacterController struct {
    useCase *usecases.CharacterUseCase
}

func NewCharacterController(useCase *usecases.CharacterUseCase) *CharacterController {
    return &CharacterController{useCase: useCase}
}

func (cc *CharacterController) CreateCharacter(w http.ResponseWriter, r *http.Request) {
    var character entities.Character
    if err := json.NewDecoder(r.Body).Decode(&character); err != nil {
        http.Error(w, err.Error(), http.StatusBadRequest)
        return
    }
    if err := cc.useCase.CreateCharacter(&character); err != nil {
        http.Error(w, err.Error(), http.StatusInternalServerError)
        return
    }
    w.WriteHeader(http.StatusCreated)
}

func (cc *CharacterController) UpdateCharacter(w http.ResponseWriter, r *http.Request) {
    var character entities.Character
    if err := json.NewDecoder(r.Body).Decode(&character); err != nil {
        http.Error(w, err.Error(), http.StatusBadRequest)
        return
    }
    if err := cc.useCase.UpdateCharacter(&character); err != nil {
        http.Error(w, err.Error(), http.StatusInternalServerError)
        return
    }
    w.WriteHeader(http.StatusOK)
}

func (cc *CharacterController) DeleteCharacter(w http.ResponseWriter, r *http.Request) {
    id := r.URL.Query().Get("id")
    if err := cc.useCase.DeleteCharacter(id); err != nil {
        http.Error(w, err.Error(), http.StatusInternalServerError)
        return
    }
    w.WriteHeader(http.StatusOK)
}

func (cc *CharacterController) GetCharacter(w http.ResponseWriter, r *http.Request) {
    id := r.URL.Query().Get("id")
    character, err := cc.useCase.GetCharacter(id)
    if err != nil {
        http.Error(w, err.Error(), http.StatusInternalServerError)
        return
    }
    if err := json.NewEncoder(w).Encode(character); err != nil {
        http.Error(w, err.Error(), http.StatusInternalServerError)
        return
    }
    w.WriteHeader(http.StatusOK)
}
```

#### `internal/interfaces/repositories/character_repository.go`
Defines the repository for character persistence.
```go
package repositories

import (
    "database/sql"
    "wasteland-chronicles/internal/entities"
)

type CharacterRepository struct {
    db *sql.DB
}

func NewCharacterRepository(db *sql.DB) *CharacterRepository {
    return &CharacterRepository{db: db}
}

func (repo *CharacterRepository) Save(character *entities.Character) error {
    // SQL insert logic
    return nil
}

func (repo *CharacterRepository) Update(character *entities.Character) error {
    // SQL update logic
    return nil
}

func (repo *CharacterRepository) Delete(id string) error {
    // SQL delete logic
    return nil
}

func (repo *CharacterRepository) FindByID(id string) (*entities.Character, error) {
    // SQL select logic
    return &entities.Character{}, nil
}
```

#### `internal/interfaces/websocket/websocket_adapter.go`
Defines the WebSocket adapter for real-time communication.
```go
package websocket

import (
    "github.com/gorilla/websocket"
    "log"
    "net/http"
)

type WebSocketAdapter struct {
    Conn *websocket.Conn
}

func NewWebSocketAdapter(w http.ResponseWriter, r *http.Request) (*WebSocketAdapter, error) {
    upgrader := websocket.Upgrader{
        CheckOrigin: func(r *http.Request) bool {
            return true
        },
    }
    conn, err := upgrader.Upgrade(w, r, nil)
    if err != nil {
        return nil, err
    }
    return &WebSocketAdapter{Conn: conn}, nil
}

func (ws *WebSocketAdapter) SendMessage(message []byte) error {
    return ws.Conn.WriteMessage(websocket.TextMessage, message)
}

func (ws *WebSocketAdapter) ReceiveMessage() ([]byte, error) {
    _, message, err := ws.Conn.ReadMessage()
    if err != nil {
        return nil, err
    }
    return message, nil
}

func (ws *WebSocketAdapter) Close() error {
    return ws.Conn.Close()
}
```

#### `internal/frameworks/database/postgres.go`
Defines the PostgreSQL database connection.
```go
package database

import (
    "database/sql"
    _ "github.com/lib/pq"
    "log"
)

func ConnectPostgres(dsn string) (*sql.DB, error) {
    db, err := sql.Open("postgres", dsn)
    if err != nil {
        return nil, err
    }
    if err := db.Ping(); err != nil {
        return nil, err
    }
    log.Println("Connected to PostgreSQL")
    return db, nil
}
```

#### `internal/frameworks/database/redis.go`
Defines the Redis connection.
```go
package database

import (
    "github.com/go-redis/redis/v8"
    "context"
    "log"
)

func ConnectRedis(addr string, password string, db int) (*redis.Client, error) {
    rdb := redis.NewClient(&redis.Options{
        Addr:     addr,
        Password: password,
        DB:       db,
    })

    ctx := context.Background()
    if err := rdb.Ping(ctx).Err(); err != nil {
        return nil, err
    }
    log.Println("Connected to Redis")
    return rdb, nil
}
```

#### `pkg/config/config.go`
Defines the configuration loader.
```go
package config

import (
    "github.com/spf13/viper"
    "log"
)

type Config struct {
    ServerPort string
    PostgresDSN string
    RedisAddr string
    RedisPassword string
    RedisDB int
}

func LoadConfig() *Config {
    viper.SetConfigName("config")
    viper.SetConfigType("yaml")
    viper.AddConfigPath(".")
    if err := viper.ReadInConfig(); err != nil {
        log.Fatalf("Error reading config file: %v", err)
    }
    return &Config{
        ServerPort: viper.GetString("server.port"),
        PostgresDSN: viper.GetString("database.postgres.dsn"),
        RedisAddr: viper.GetString("database.redis.addr"),
        RedisPassword: viper.GetString("database.redis.password"),
        RedisDB: viper.GetInt("database.redis.db"),
    }
}
```

#### `pkg/middleware/auth.go`
Defines the authentication middleware.
```go
package middleware

import (
    "net/http"
)

func AuthMiddleware(next http.Handler) http.Handler {
    return http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
        // Authentication logic
        next.ServeHTTP(w, r)
    })
}
```

#### `pkg/utils/validation.go`
Defines utility functions for input validation.
```go
package utils

import "regexp"

func ValidateEmail(email string) bool {
    re := regexp.MustCompile(`^[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$`)
    return re.MatchString(email)
}
```

### Additional Considerations
1. **Error Handling:** Ensure proper error handling and logging throughout the code.
2. **Testing:** Write unit tests for each layer to ensure functionality.
3. **Security:** Implement security measures such as authentication, authorization, and data encryption.
4. **Documentation:** Document the API endpoints, data structures, and business logic.
5. **Scalability:** Implement horizontal scaling and use containerization for easier deployment.

This structure provides a solid foundation for building the backend of "Wasteland Chronicles" using Go and WebSockets, following Clean Architecture principles. Each layer has a clear responsibility, making the codebase easier to maintain and scale.
