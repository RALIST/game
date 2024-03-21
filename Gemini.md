## Wasteland Chronicles: Full Game Design Document (GDD) - Final Version (All Parts)

**Part 1: Introduction and Overview**

**Game Title:** Wasteland Chronicles

**Genre:** Text-based MMORPG with strategy elements

**Target Platform(s):** Web browser, Telegram Mini Apps

**Target Audience:** Fans of Fallout and post-apocalyptic settings, MMORPG players who enjoy text-based experiences and collaborative gameplay.

**Project Goals:**

- Create an engaging and immersive text-based MMORPG that captures the essence of the Fallout universe.
    
- Foster a strong sense of community through cooperative gameplay and shared goals.
    
- Offer a unique blend of strategy, character development, and exploration in a text-based format.
    
- Provide a platform for roleplaying and player-driven storytelling within the game world.
    

**Project Scope:**

The initial scope focuses on developing the core gameplay loop, including:

- Character creation and development using the S.P.E.C.I.A.L. system, skills, perks, and traits.
    
- Exploration and resource gathering in the diverse regions of the wasteland.
    
- Crafting of weapons, armor, tools, and consumables using blueprints and modifications.
    
- Collaborative settlement building and management, including a voting system for prioritizing structures.
    
- Turn-based combat against hostile creatures and raiders.
    
- Social interaction and trading between players.
    

Future expansions may include:

- Guilds and player factions for deeper social interaction and competition.
    
- Player-versus-player (PvP) and expanded cooperative gameplay elements.
    
- More complex crafting systems with additional blueprints and modifications.
    
- Deeper settlement management with resource production, population growth, and defense mechanics.
    
- Expansion of the world and lore through additional quests, events, and storylines.
    

**Game Overview:**

**Game Concept:**

Wasteland Chronicles is a text-based MMORPG set in a post-apocalyptic world inspired by the Fallout universe. Players cooperate to rebuild society and survive in a harsh and dangerous environment. A unique threat, the poisonous cloud, periodically sweeps across the land, forcing players to work together to construct a shelter and protect their settlement.

**Unique Selling Proposition (USP):**

Wasteland Chronicles offers a unique blend of text-based MMORPG experience with strategic settlement building and resource management. The game emphasizes player cooperation and community decision-making through its voting system, creating a shared sense of purpose and responsibility. The ever-present threat of the poisonous cloud adds tension and urgency to the gameplay, encouraging players to work together and prioritize the settlement's survival.

**Compelling Hook:**

"In the shadow of the poisonous cloud, forge your destiny in the wasteland. Will you scavenge for survival, build a thriving community, or conquer your rivals? The choice is yours in Wasteland Chronicles, a text-based MMORPG where your actions shape the future of your settlement."

**Part 2: Game Mechanics - Character System**

- **S.P.E.C.I.A.L. System:**
    
    - Players allocate 40 points among the 7 attributes during character creation.
        
    - Each attribute point increases the relevant stat by 1 and affects various gameplay aspects:
        
        - **Strength:** Increases melee damage by 5% per point and carrying capacity by 10 lbs per point.
            
        - **Perception:** Increases ranged weapon accuracy by 2% per point and the chance to detect hidden objects.
            
        - **Endurance:** Grants 10 starting health points per point, increases resistance to radiation and poison, and affects fatigue accumulation.
            
        - **Charisma:** Influences NPC interactions, bartering prices (1% discount/increase per point), persuasion attempts, and skills like Speech and Leadership.
            
        - **Intelligence:** Grants an additional skill point every 2 levels per point, allows for crafting more complex items, affects hacking success rates, and influences skills like Science and Medicine.
            
        - **Agility:** Grants an additional action point in combat for every 2 points above 5, increases movement speed on the world map, improves stealth capabilities, and affects skills like Sneak and Guns.
            
        - **Luck:** Increases critical hit chance by 1% per point, influences random encounter outcomes, increases the chance of finding better loot, and provides a small bonus to all skills.
            
- **Skills:**
    
    - Skills are categorized into Combat, Crafting, and Social categories.
        
    - Examples include:
        
        - **Combat:** Small Guns, Big Guns, Melee Weapons, Unarmed, Explosives, Energy Weapons.
            
        - **Crafting:** Repair, Science, Medicine, Engineering, Cooking.
            
        - **Social:** Speech, Barter, Gambling, Persuasion, Leadership.
            
    - Each skill starts at level 0 and can be increased to a maximum of 100 using skill points gained through level-ups (3 points per level).
        
    - Certain perks can provide bonuses to specific skills (e.g., "Gunslinger" perk grants +10 to Small Guns skill).
        
    - Skill checks are performed using a dice roll system (1d100). The player needs to roll equal to or below their skill level to succeed.
        
    - Skill specializations can be chosen within each category at levels 5 and 10, providing additional bonuses and abilities related to the chosen focus.
        
- **Perks:**
    
    - Perks are unlocked every 2 levels, starting at level 2, and some require specific skill levels or other prerequisites.
        
    - Perks are categorized into three tiers with increasing power and stricter prerequisites:
        
        - Tier 1 (Levels 2, 4, 6, etc.): Basic perks like "Strong Back" (increased carrying capacity) or "First Aid" (improved healing effectiveness).
            
        - Tier 2 (Levels 8, 10, 12, etc.): More powerful perks like "Sniper" (increased ranged accuracy and critical chance) or "Chemist" (craft more potent drugs).
            
        - Tier 3 (Levels 14, 16, 18, etc.): Highly specialized perks like "Robotics Expert" (control robots) or "Mastermind" (increased influence and persuasion).
            
    - Perk trees can branch out based on character choices and specializations, allowing for deeper customization and unique builds.
        
- **Traits:**
    
    - Players can choose up to 2 traits during character creation.
        
    - Traits provide significant advantages and disadvantages, encouraging roleplaying and strategic character builds.
        
    - Traits can have synergistic effects with specific perks or skills, further enhancing character specialization.
        
    - Examples:
        
        - "Fast Metabolism" increases health regeneration by 50% but also increases hunger and thirst rates by 20%.
            
        - "Gifted" grants +1 Intelligence and a bonus to Science skill checks.
            
        - "Lone Wanderer" grants combat bonuses, faster movement, and increased resource gathering efficiency when alone, but applies penalties when in groups.
            

**Part 3: Game Mechanics - Wasteland Exploration**

- **World Map:**
    
    - The map is divided into 5 regions with increasing difficulty and resource rarity:
        
        - Starting Region: Safe haven with basic resources.
            
        - Ruined City: Moderate danger with opportunities for advanced loot.
            
        - Radioactive Wasteland: High radiation levels and mutated creatures.
            
        - Forgotten Bunker: Challenging puzzles and pre-war technology.
            
        - Hidden Oasis: Rare resources guarded by powerful enemies.
            
    - Travel time between regions is calculated based on distance and character Agility (1 hour per region base, reduced by 10% per point in Agility).
        
    - Random encounter chance is 20% per region traveled, with higher difficulty regions having a higher chance for more dangerous encounters.
        
- **Locations:**
    
    - Each region has 10 unique locations with specific descriptions, available resources, and potential quests or events.
        
    - Resource gathering nodes respawn every 24 hours (real-time) and provide materials based on the region's difficulty and the type of node.
        
    - Location-specific quests and events provide various rewards, including experience points, bottle caps, unique items, and reputation gains with specific factions.
        
- **Combat:**
    
    - Turn-based combat system with action points (AP) determining the number of actions per turn.
        
    - AP is determined by Agility (2 base AP + 1 AP per 2 points in Agility above 5) and can be further increased by perks.
        
    - Weapon damage is calculated based on weapon type, Strength, and relevant skill level.
        
    - Critical hits deal 1.5x normal damage and have a base chance of 5%, increased by Luck and specific weapon types/perks.
        
    - Combat actions and tactics include melee attacks, ranged attacks, special abilities granted by perks, and the use of consumables like grenades or stimpaks.
        
    - Enemy AI and tactics vary depending on the enemy type, providing a dynamic combat experience.
        
    - Damage calculation takes into account weapon base damage, Strength and skill modifiers, armor reduction, and critical hits.
        
    - Status effects like bleeding, poisoning, radiation sickness, and stunning can be applied in combat and have various impacts on character stats and actions.
        
    - Combat difficulty scales based on player level, group size, and dynamic adjustments based on player performance.
        

**Part 4: Game Mechanics - Crafting System**

- **Crafting Stations:**
    
    - Different crafting stations are required for different types of crafting (e.g., Workbench for weapons and armor, Chemistry Station for drugs and explosives).
        
    - Upgraded stations unlock more complex crafting recipes and modifications.
        
    - Each station has specific resource requirements for building and upgrading.
        
- **Blueprints:**
    
    - Over 50 unique blueprints can be found or purchased, covering various item types like weapons, armor, tools, and consumables.
        
    - Blueprint complexity determines the required skill level and material cost for crafting.
        
- **Modifications:**
    
    - Each weapon and armor piece can have up to 3 modifications installed.
        
    - Modifications provide various bonuses, such as increased damage, accuracy, or armor rating.
        
    - Installing modifications requires specific materials and skill levels.
        

**Part 5: Game Mechanics - Settlement Building**

- **Building Types:**
    
    - 10 different building types are available, each with unique functions and upgrade paths.
        
    - Building costs and construction times scale with complexity and upgrade level.
        
    - Buildings interact with each other to create a dynamic settlement system. For example, higher-level farms provide more food, which increases happiness and workforce availability.
        
- **Voting System:**
    
    - Each player gets one vote per day for the building they want to prioritize.
        
    - Players can campaign and debate to influence others' votes.
        
    - The building with the most votes receives a 20% construction progress bonus.
        
- **Building Upgrades:**
    
    - Each building has 3 upgrade levels, unlocking new features and increasing efficiency.
        
    - Upgrades require specific resources and may depend on research progress in the Research Lab.
        
- **Settlement Management:**
    
    - Players manage resources, population, happiness, and defenses within the settlement.
        
    - This includes resource allocation, job assignments for NPCs, and responding to threats like raider attacks.
        
    - Defensive structures provide both passive and active defense during attacks, with higher levels offering greater protection and offensive capabilities.
        

**Part 6: Game Mechanics - Economy and Trade**

- **Currency:**
    
    - Bottle caps are the primary currency, with rarer items like pre-war money having higher value (1 pre-war dollar = 100 bottle caps).
        
    - Bartering skill and charisma can influence trade prices by up to 20%.
        
- **Player Trading:**
    
    - Players can set up personal shops in the settlement marketplace to sell items for bottle caps or barter with other players.
        
    - Direct trading between players allows for negotiation and customized deals.
        
- **Shop:**
    
    - The settlement shop offers only basic items required for starting out and establishing basic farming operations. Advanced items can only be acquired through crafting.
        

**Part 7: Game Mechanics - Additional Mechanics**

- **Quests:**
    
    - Over 30 quests are available, ranging from simple fetch quests to complex story-driven missions.
        
    - Quest rewards include experience, bottle caps, unique items, and reputation gains.
        
    - Quests are categorized into main story quests, side quests, faction quests, and repeatable quests.
        
    - Quests offer meaningful choices that can impact the game world and narrative, with some offering branching paths and different outcomes.
        
- **Factions and Reputation:**
    
    - 5 major factions exist in the wasteland, each with its own ideology and goals.
        
    - Reputation with factions affects interactions with their members and opens up faction-specific quests and rewards.
        
- **Events:**
    
    - Over 20 random events can occur, ranging from finding a hidden cache to defending the settlement from raiders.
        
    - Event outcomes can be influenced by player choices and actions.
        
    - Events can have various impacts on gameplay, such as providing opportunities for acquiring rare resources or items, introducing new challenges, affecting reputation, and triggering dynamic changes in the game world.
        
- **Social Interaction:**
    
    - Players can chat publicly or privately, form groups, and engage in roleplay.
        
    - Group activities can provide bonuses to experience gain and resource gathering.
        
    - The user interface includes specific elements and functionalities for chat, group management, and trading.
        

**Part 8: Game World**

- **World Map:**
    
    - The wasteland is divided into 5 distinct regions with increasing difficulty and resource rarity:
        
        - Starting Region: Safe haven with basic resources.
            
        - Ruined City: Moderate danger with opportunities for advanced loot.
            
        - Radioactive Wasteland: High radiation levels and mutated creatures.
            
        - Forgotten Bunker: Challenging puzzles and pre-war technology.
            
        - Hidden Oasis: Rare resources guarded by powerful enemies.
            
- **Locations:**
    
    - Each region contains 10 unique locations with specific descriptions, available resources, and potential quests or events.
        
- **Factions and NPCs:**
    
    - Several factions with unique ideologies and goals inhabit the wasteland.
        
    - NPCs within these factions offer quests, trade opportunities, and lore insights.
        
    - Players can build relationships with NPCs by completing quests, trading fairly, and making choices that align with the faction's ideology.
        
- **Lore and Story:**
    
    - Wasteland Chronicles is set in a post-apocalyptic world where the remnants of society struggle to rebuild after a devastating nuclear war.
        
    - The poisonous cloud, a byproduct of the war's environmental destruction, periodically sweeps across the land, posing a constant threat to survival.
        
    - Players uncover the history of the world, the cause of the apocalypse, and the secrets of the poisonous cloud through exploration, quests, and interactions with NPCs.
        

**Part 9: User Interface and Controls**

- **Interface Design:**
    
    - Text-based interface with menus, descriptions, and interactive commands.
        
    - Detailed mockups or wireframes show the layout and organization of UI elements.
        
- **Navigation and Menus:**
    
    - Players navigate through menus using simple text commands and keywords.
        
    - Context-sensitive commands are available within each menu for specific interactions.
        
- **Controls and Input:**
    
    - Players primarily use text commands and keywords to interact with the game world.
        
    - The game recognizes a variety of synonyms and abbreviations for commands.
        
- **Feedback and Information Display:**
    
    - Detailed descriptions provide feedback on actions and immerse players in the world.
        
    - The UI displays information about character stats, inventory, crafting, settlement status, and other relevant game elements.
        
- **Error Handling and Feedback:**
    
    - The UI provides clear and informative feedback to players when actions fail or encounter issues, including specific error messages, visual/audio cues, and suggestions for alternative actions.
        
- **Social Interaction Features:**
    
    - The UI includes specific elements and functionalities for chat, group management, and trading.
        

**Part 10: Technical Specifications**

- **Game Engine:** Node.js / Typescript for server-side logic and Redis for data storage.
    
- **Programming Language(s):** TypeScript for both server and client-side development.
    
- **Art Style and Assets:** While primarily text-based, the game may incorporate stylized visuals for maps, character portraits, and key items.
    
- **Sound Design and Music:** Atmospheric soundscapes and music enhance the game's immersion and setting.
    
- **Network and Multiplayer:** WebSocket protocol enables real-time communication and interaction between players.
    
- **Backend Architecture:**
    
    - Detailed overview of how different modules interact and how data is stored and managed using Redis and a persistent database.
        
    - **Event-Based Asynchronous Architecture:** Redis Streams are used to implement an event-based asynchronous architecture on the backend, allowing for efficient handling of concurrent actions and inter-module communication.
        
- **API Design:**
    
    - Definition of APIs used for communication between the backend and frontend, specifying the data structures and protocols used for exchanging information.
        
- **Scalability and Performance Considerations:**
    
    - Strategies for ensuring the game's scalability and performance with a large number of players and concurrent actions, including efficient data structures, caching mechanisms, and load balancing techniques.
        
- **Data Persistence:**
    
    - Game data is persisted using a combination of Redis for real-time data and a persistent database (e.g., MongoDB) for long-term storage.
        
- **Security Measures:**
    
    - Data validation, encryption, and user authentication protocols are implemented to protect game data and prevent cheating or malicious activity.
        

**Part 11: Development Roadmap**

- **Phase 1: Core Gameplay Development:**
    
    - Implement the core gameplay loop, including character creation, exploration, crafting, settlement building, combat, and basic social interaction.
        
    - Focus on building a functional and enjoyable prototype of the main gameplay mechanics.
        
- **Phase 2: Content Expansion and Refinement:**
    
    - Expand the game world with additional locations, quests, events, and lore.
        
    - Refine existing mechanics based on player feedback gathered from playtesting the prototype.
        
- **Phase 3: Advanced Features and Polishing:**
    
    - Implement advanced features like guilds, PvP, and deeper settlement management.
        
    - Polish the game, addressing bugs and balancing gameplay elements.
        
    - Prepare marketing materials and launch the game on the chosen platforms.
        

**Part 12: Marketing and Publishing**

- **Target Market:** Focus on fans of Fallout, post-apocalyptic settings, and text-based MMORPGs.
    
- **Marketing Strategy:** Utilize social media, online forums, and targeted advertising to reach the target audience. Build a strong community through regular communication and engaging content.
    
- **Publishing Plan:** Self-publish on web browser and Telegram Mini Apps platforms.
    
- **Monetization Model:** Consider an optional subscription model or in-game purchases for cosmetic items or convenience features.
    

**Part 13: Conclusion**

Wasteland Chronicles aims to offer a unique and engaging text-based MMORPG experience that emphasizes community building, strategic decision-making, and exploration in a post-apocalyptic world. By focusing on strong writing, detailed descriptions, and engaging gameplay mechanics, the game will immerse players in its world and foster a strong sense of community. The development roadmap prioritizes building a solid foundation for the core gameplay loop before expanding with additional features and content. With a focused marketing strategy and accessible publishing plan, Wasteland Chronicles has the potential to attract a dedicated player base and carve out its own niche in the MMORPG landscape.