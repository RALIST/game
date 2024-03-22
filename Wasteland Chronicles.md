# Game Design Document (GDD)

## Part 1: Introduction and Overview

### Overview

**Game Title:** Wasteland Chronicles  
**Genre:** Text-based MMORPG with strategy elements  
**Target Platforms:** Telegram Mini Apps  
**Target Audience:** Fans of Fallout and post-apocalyptic settings, MMORPG players who enjoy text-based experiences and collaborative gameplay.
### Project Goals

- Create an engaging and immersive text-based MMORPG that captures the essence of the Fallout universe.
- Foster a strong sense of community through cooperative gameplay and shared goals.
- Offer a unique blend of strategy, character development, and exploration in a text-based format.
- Provide a platform for roleplaying and player-driven storytelling.
### Project Scope

The initial scope focuses on developing the core gameplay loop, including:
- Character creation and development using the S.P.E.C.I.A.L. system, skills, perks, and traits.
- Exploration and resource gathering in the diverse regions of the wasteland.
- Crafting of weapons, armor, tools, and consumables using blueprints and modifications.
- Collaborative settlement building and management, including a voting system for prioritizing structures.
- Turn-based combat against hostile creatures and raiders.
- Social interaction and trading between players.

**Future expansions may include:**
- Guilds and player factions.
- Player-versus-player (PvP) and expanded cooperative gameplay elements.
- More complex crafting systems.
- Deeper settlement management with resource production, population growth, and defense mechanics.
- Expansion of the world and lore.
### Game Overview

Wasteland Chronicles is a text-based MMORPG set in a post-apocalyptic world inspired by the Fallout universe. Players cooperate to rebuild society and survive in a harsh and dangerous environment, facing the ever-present threat of a poisonous cloud that periodically sweeps across the land.
#### Unique Selling Proposition (USP)

Wasteland Chronicles offers a unique blend of text-based MMORPG experience with strategic settlement building and resource management. The game emphasizes player cooperation and community decision-making through its voting system, creating a shared sense of purpose and responsibility. The ever-present threat of the poisonous cloud adds tension and urgency to the gameplay, encouraging players to work together and prioritize the settlement's survival.
#### Compelling Hook

"In the shadow of the poisonous cloud, forge your destiny in the wasteland. Will you scavenge for survival, build a thriving community, or conquer your rivals? The choice is yours in Wasteland Chronicles, a text-based MMORPG where your actions shape the future of your settlement."
## Part 2: Character System

### Attributes

#### Strength
- Affects physical damage dealt in melee combat.
- Determines carrying capacity.
- Influences success in Strength-based skill checks (e.g., breaking down doors).
#### Perception
- Influences accuracy with ranged weapons.
- Affects awareness of surroundings and enemy detection.
- Determines success in Perception-based skill checks (e.g., spotting hidden objects).
#### Endurance
- Determines maximum health points (HP).
- Influences resistance to damage and radiation.
- Affects physical resilience and fatigue recovery.
#### Charisma
    - Influences interactions with NPCs and persuasion attempts.
    - Affects prices in bartering and trading.
    - Determines success in Charisma-based skill checks (e.g., leading a group).
#### Intelligence
- Determines the number of skill points gained per level.
- Influences success in Science and Medicine skills.
- Affects understanding of lore and technology.
#### Agility
- Determines Action Points (AP) available in combat.
- Influences movement speed and evasion.
- Determines success in Agility-based skill checks (e.g., sneaking).
#### Luck
- Influences critical hit chance in combat.
- Affects the outcome of random encounters and events.
- Determines success in Luck-based skill checks (e.g., gambling).

Each attribute point increases the relevant stat by 1 and affects various gameplay aspects, such as combat damage, skill checks, carrying capacity, and interaction with NPCs.

### Stats:
#### Maximum Health Points (HP)
Determined by Endurance. Represents the character's overall health and ability to withstand damage.
#### Action Points (AP)
Determined by Agility. Used to perform actions in combat, such as attacking, moving, or using items.
#### Carrying Capacity 
Determined by Strength. Limits the amount of weight the character can carry.
#### Healing Rate
Influences how quickly the character recovers health points (HP) over time.
Affected by Endurance and the Medicine skill.
Can be further increased by perks, consumables, and medical facilities within settlements.
The recovery rate being significantly higher when the character is resting in their house.
#### Critical Chance
Represents the chance to land a critical hit in combat, dealing increased damage.
Affected by Luck and specific combat skills (e.g., Sniper perk for ranged weapons).
Can be further increased by perks, equipment modifications, and consumables.
#### Radiation Resistance
Determines the character's resistance to radiation exposure.
Affected by Endurance and can be further increased by perks
#### Reputation
Represents the character's standing with settlement
Can be decreased by actions against settlement (stealing and so on).
Can be descreased by other players.
Higher reputation unlocks unique rewards, special services and options in settlement. Also player's voting power huge depends  on reputation
#### Karma
Represents the character's overall moral compass
Can be increased by helping others, showing mercy, and making selfless decisions.
Can be decreased by harming innocents, stealing, and making cruel or selfish choices.
Karma can influence NPC interactions, quest outcomes, trigger specific encounters.
#### Fatigue
Represents the character's level of exhaustion and affects their overall performance.
Increases with various activities, including exploring routes, crafting. Higher fatigue levels can lead to:
   - Reduced combat effectiveness (e.g., lower accuracy, damage output, and AP regeneration).
  - Decreased crafting efficiency (e.g., longer crafting times, increased resource costs).
  - Slower movement speed during exploration.
  Fatigue recovers over time, with the recovery rate being significantly higher when the character is resting in their house.
Consumables and specific perks can also help reduce fatigue or increase its recovery rate.
##### Balancing notes
- The rate at which fatigue accumulates should be balanced to prevent players from feeling overly restricted while still encouraging breaks and strategic gameplay.
- The fatigue recovery rate in player houses should be significant enough to incentivize players to utilize their houses for rest and recovery.
- Different activities should contribute to fatigue at varying rates, with more strenuous activities like combat causing faster fatigue accumulation.
#### Level
Just a player's level
#### Experience (XP)
Current player's experience

### Skills
#### ==Combat==
##### Ranged Weapons
Governs the use of all ranged weapons, including pistols, rifles, SMGs, miniguns, rocket launchers, flamethrowers, laser weapons, and plasma weapons. Higher levels increase accuracy, damage, critical hit chance, and unlock special combat maneuvers and weapon-specific attacks, including energy-based abilities.
##### Melee Weapons
Governs the use of melee weapons and unarmed. Higher levels increase damage, critical hit chance, and unlock special attacks like disarming strikes or power attacks.
#### ==Crafting==
##### Repair
Allows for repairing weapons, armor, and tools. Higher skill levels allow for repairing more complex items.
##### Science
Used for crafting advanced items and researching new technologies. Higher skill levels unlock more complex recipes and research projects.
##### Medicine
Allows for healing injuries and crafting medical supplies. Higher skill levels improve healing effectiveness and unlock advanced medical procedures.
##### Engineering
Used for building and upgrading structures in the settlement. Higher skill levels unlock more advanced structures and upgrades.

High level crafting skills allow for experimentation and improvisation, enabling players to create unique modifications or even entirely new items
#### ==Social==

##### Speech
Influences NPC interactions and persuasion attempts. Higher skill levels unlock unique dialogue options and increase persuasion success.
##### Barter
Affects trade prices and negotiation success. Higher skill levels lead to better deals and more profitable trades.
##### Gambling
Used for playing games of chance and winning bottle caps. Higher skill levels increase the chance of winning.
##### Persuasion
Influences NPC interactions and quest outcomes. Higher skill levels unlock additional quest options and influence NPC behavior.
##### Leadership
Provides bonuses to group activities and settlement management. Higher skill levels improve group morale, productivity, and settlement efficiency.
### Perks

Perks are unlocked every 2 levels, starting at level 2, and some require specific skill levels or other prerequisites.

Perks are categorized into three tiers with increasing power and stricter prerequisites:

- **Tier 1:** (Unlocked at level 2, no prerequisites)
    - **Strong Back:** Increases carrying capacity.
    - **First Aid:** Improves healing effectiveness.
    - **Gunslinger:** Increases accuracy with pistols.
    - **Commando:** Increases accuracy with automatic weapons.
    - **Iron Fist:** Increases damage with unarmed and melee weapons.
- **Tier 2:** (Unlocked at level 4, requires specific skill levels)
    - **Sniper:** (Requires Ranged Weapons: Adept) Increases ranged accuracy and critical chance.
    - **Chemist:** (Requires Medicine: Adept) Craft more potent drugs and medical supplies.
    - **Architect:** (Requires Engineering: Adept) Unlocks advanced building options and reduces construction costs.
    - **Silver Tongue:** (Requires Speech: Adept) Increases persuasion success and unlocks unique dialogue options.

- **Tier 3:** (Unlocked at level 6, requires specific skill levels and/or quest completion)
    - **Robotics Expert:** (Requires Science: Expert) Allows for hacking and controlling robots.
    - **Mastermind:** (Requires Leadership: Expert) Increases influence and persuasion, provides bonuses to group activities.
    - **Survivalist:** (Requires Endurance: Expert and completion of a specific survival-themed quest) Increases resistance to radiation and harsh environments.

Perk trees can branch out based on character choices and specializations, allowing for deeper customization and unique builds.

**Additional Perks:** Some perks could require completing challenging or hidden achievements, encouraging exploration and experimentation.

### Traits
 Players can choose up to 2 traits during character creation, providing significant advantages and disadvantages.
Traits can have synergistic effects with specific perks or skills.
- **Gifted:** (Intelligence +1, Luck -1)
- **Strong Back:** (Strength +2, Agility -1)
- **Fast Metabolism:** (Endurance +1, heals faster, but requires more food)
- **Bruiser:** (Strength +1, Endurance +1, Intelligence -1)
- **Savvy:** (Perception +2, Charisma -1)
### Character Advancement

- Characters gain experience points (XP) by completing quests, defeating enemies, crafting items, and participating in settlement activities.
- Upon reaching certain XP thresholds, characters level up.
- Each level grants the player attribute points and skill points for further character development and customization.
### Mutations

- Exposure to radiation or other environmental hazards could cause mutations, which can have both positive and negative effects on the character.
- Players could choose to embrace mutations or seek ways to cure them, depending on their desired playstyle and roleplaying preferences.
## Part 3:  Wasteland Exploration

### Game world

#### Lore and Story

- Wasteland Chronicles is set in a post-apocalyptic world where the remnants of society struggle to rebuild after a devastating nuclear war.
- The game world is filled with remnants of the past, offering clues about the events that led to the apocalypse and the state of the world before the war.
- The poisonous cloud, a byproduct of the war's environmental destruction, periodically sweeps across the land, posing a constant threat to survival.
- Players uncover the history of the world, the cause of the apocalypse, and the secrets of the poisonous cloud through exploration, quests, and interactions with NPCs.
### Dynamic World Events

Introduce large scale events that impact the entire game world, requiring players to collaborate and adapt

- **Weather Anomalies:** A sudden and severe dust storm or radioactive storm sweeps across the wasteland, impacting travel, resource gathering, and combat.
- **Faction Conflicts:** War erupts between major factions, changing the political landscape and creating new opportunities and dangers for players.
- **Emergence of New Threats:** A new and powerful enemy emerges in the wasteland, requiring players to band together and find ways to defeat it.

These dynamic events keep the game world feeling alive and unpredictable, requiring players to adapt their strategies and work together to overcome new challenges.

Integrate lore elements into the game world through environmental storytelling, quest dialogues, and NPC interactions.

Players can uncover the history of the world, the cause of the apocalypse, and the secrets of thepoisonous cloud through exploration, quests, and interactions with NPCs.

Hidden secrets and puzzles within locations can reveal lore, provide access to rare resources, or unlock special encounters.
### Routes

- The wasteland is divided into 5 distinct routes with increasing difficulty and resource rarity:
  - **Route to the Safe Haven:** This route leads to a small, fortified settlement that serves as a safe haven for travelers and traders. It provides basic resources, shelter, and opportunities for trade. This route is relatively safe and serves as a starting point for new players.
  - **Route to the Ruined City:** This route leads to the ruins of a once-thriving city. The city is now filled with dangers, but also holds opportunities for finding advanced loot and remnants of pre-war technology. This route is more challenging than the Safe Haven route and offers greater rewards for experienced players.
  - **Route to the Radioactive Wasteland:** This route leads to a desolate wasteland with high levels of radiation. Mutated creatures roam the wasteland, and resources are scarce. However, this route also holds the potential for finding rare and valuable materials needed for crafting powerful items. This route is very dangerous and requires careful preparation and protective gear.
 - **Route to the Forgotten Bunker:** This route leads to a hidden pre-war bunker that has been forgotten by most wasteland inhabitants. The bunker contains valuable technology and information about the past, but it is also protected by challenging puzzles and security systems. This route requires problem-solving skills and combat prowess to overcome the obstacles and access the bunker's secrets.
  - **Route to the Hidden Oasis:** This route leads to a lush and vibrant oasis hidden within the wasteland. The oasis offers rare resources and a respite from the harsh environment, but it is also guarded by powerful enemies. This route is the most challenging and requires a high level of skill and preparation to overcome the dangers and reap the rewards of the oasis.
As players explore the wasteland and complete quests, they can find special items that reveal information about new routes:

 - **Old books:** These books might contain forgotten knowledge about pre-war locations or hidden paths through the wasteland.
 - **Maps:** These maps might show the locations of secret bunkers, hidden oases, or other valuable destinations.
- **Hard drives:** These hard drives might contain pre-war data with coordinates or information about secret facilities or hidden caches.
 Upon finding and deciphering these items, players can unlock new routes on the world map, expanding their exploration options and leading them to new challenges and rewards.

#### Locations

- Each route contains 10 unique locations with specific descriptions, available resources, and potential quests or events.
- Each location has its own distinct theme and atmosphere, providing diverse environments for players to explore.
- Each location could have hidden secrets or puzzles that reveal lore, provide access to rare resources, or unlock special encounters.

**Narrative Justification:**

- The routes are established and maintained by experienced wasteland travelers and traders.
- They represent the safest and quickest paths to reach specific destinations, avoiding unnecessary dangers and obstacles.
- Due to the harsh conditions of the wasteland, traveling off the established routes is considered extremely dangerous and is not recommended for most travelers.

**Example routes to unlock (Examples):**

- **Route to the Pre-War Military Base:** This route can be unlocked by finding a map hidden in the Ruined City. The military base contains valuable pre-war technology, weapons, and information, but it is also heavily guarded by automated defenses and powerful robots.
- **Route to the Secret Research Facility:** This route can be unlocked by completing a quest for a specific faction. The research facility contains advanced scientific equipment and research data that can be used to develop new technologies and upgrades for settlements.
- **Route to the Lost Vault:** This route can be unlocked by deciphering a hard drive found in the Forgotten Bunker. The Lost Vault is a legendary pre-war vault that is rumored to contain vast riches and advanced technology. However, it is also said to be protected by deadly traps and security systems.
### Group Completion

- Players can form groups to complete routes together, combining their skills and resources to overcome challenges more effectively.
- Group completion can provide bonuses to experience gain and resource gathering, encouraging cooperative gameplay.
- **Clarification:** All players in the group need to be present at the final location to complete the route and share the rewards.
### Death Mechanics

- If a player dies during a route, they will lose all or part of their equipment.
- The amount of equipment lost can depend on the difficulty of the route and the circumstances of the player's death.
- Players can return to the location where they died to retrieve their lost equipment, but there is a risk that other players might have looted it before they return.
- **Clarification:** Equipment loss upon death will be balanced to avoid being overly punishing while still maintaining a sense of risk and consequence.
### Return Timers

- After completing the last location on a route, players can return to their base without having to visit all locations in reverse order.
- This can be done by activating a return timer, which will teleport the player back to their base after a certain amount of time.
- The duration of the return timer can depend on the length and difficulty of the route.
- **Clarification:** The return timer duration will be balanced to prevent players from easily bypassing challenges but not be so long that it becomes tedious or frustrating.

**Suggestions for Future Consideration:**

- **Separate Solo and Group Routes:** Separate routes could be designed specifically for solo play and group play. This would allow for tailored challenges and rewards for each type of gameplay experience.

## Part 4: Combat System

### Turn-Based Combat

- Wasteland Chronicles utilizes a turn-based combat system with Action Points (AP) determining the number of actions a character can take per turn.
- AP is influenced by the character's Agility attribute and can be further modified by perks and equipment.
- Players can choose from various combat actions, such as:
    - **Attack:** Basic attack with equipped weapon, consuming AP based on weapon type and attack type (e.g., aimed shot consuming more AP than a regular shot).
    - **Special Attacks:** Specific attacks unlocked by skills or perks, such as power attacks, disarming strikes, or energy-based abilities.
    - **Defense:** Enter a defensive stance, increasing damage resistance and reducing incoming damage.
    - **Movement:** Move around the battlefield, consuming AP based on distance and terrain.

    - **Use Items:** Use consumables like stimpaks or grenades during combat.

    - **Reload:** Reload ranged weapons, consuming AP based on weapon type.

- Critical hits deal increased damage and have a chance to inflict additional effects, such as bleeding or stunning.
- Combat ends when all enemies are defeated or the player's party is incapacitated.
### Enemy Types
- Wasteland Chronicles features a variety of enemy types with different strengths, weaknesses, and combat tactics:
    - **Raiders:** Human enemies equipped with various weapons and armor.
    - **Mutants:** Creatures mutated by radiation, often possessing enhanced strength and resilience.
    - **Robots:** Pre-war robots with advanced weaponry and defenses.
    - **Animals:** Hostile animals found in the wasteland, such as mutated rats, radscorpions, or deathclaws.

- Each enemy type has unique attack patterns and behaviors, requiring players to adapt their tactics accordingly.
- Some enemies may have special abilities or resistances, adding further complexity to combat encounters.
### Combat Difficulty

- Combat difficulty scales with the player's level and group size, ensuring challenging encounters throughout the game.
- Players can adjust the difficulty level to customize their experience.
- Higher difficulty levels offer greater rewards but also pose a greater risk of failure and character death.
### Combat Strategies

- Players can employ various strategies to gain an advantage in combat:

    - **Positioning:** Utilize cover and flanking maneuvers to gain tactical advantages.
    - **Targeting:** Prioritize high-threat enemies or focus fire on specific targets.
    - **Skill Synergies:** Combine different skills and perks to create powerful combos and maximize damage output.
    - **Consumables:** Use consumables strategically to heal, buff allies, or cripple enemies.
### Additional Combat Mechanics

- **Stealth:** Players can utilize stealth to avoid combat encounters or gain a surprise attack advantage.
- **Environmental Hazards:** Combat encounters can take place in environments with hazards that can be used to the player's advantage, such as explosive barrels or radioactive zones.
- **Companion System:** Players may be able to recruit companions who can assist them in combat, providing additional firepower and support.

## Part 5:  Crafting System

### Crafting Stations

Different crafting stations are required for different types of crafting:
- **Workbench:** Used for crafting and modifying weapons, armor, and tools.
- **Chemistry Station:** Used for crafting drugs, medical supplies, and explosives.
- **Research Lab:** Used for researching new technologies and blueprints.

Additional stations can be added in future expansions, such as a Robotics Station for crafting and repairing robots.
Upgraded stations unlock more complex crafting recipes and modifications. Upgrading stations requires resources and might depend on research progress in the Research Lab.
Each station has specific resource requirements for building and upgrading.
### Blueprints

Over 50 unique blueprints can be found or purchased, covering various item types like weapons, armor, tools, and consumables.
- Blueprints provide the instructions and specifications for crafting specific items.
- Blueprint complexity determines the required skill level and material cost for crafting.
- Include rare and powerful recipes that require ingredients found only in dangerous locations or acquired through complex quests.
#### Blueprint Acquisition
- **Found:** Blueprints can be found while exploring the wasteland, often in hidden caches or abandoned buildings.
- **Purchased:** Blueprints can be purchased from merchants or traders in settlements.
- **Researched:** High-level Research Labs in settlements can allow players to research and unlock new blueprints.
### Modifications

Each weapon and armor piece can have up to 3 modifications installed.
Each modification slot can accommodate a specific type of modification (e.g., one slot for sights, one for barrels, and one for stocks on a weapon).
Modifications provide various bonuses, such as increased damage, accuracy, or armor rating. They can also add unique effects or properties to items, such as increased critical hit chance, reduced recoil, or elemental damage.
Installing modifications requires specific materials and skill levels.
Implement a system of material quality tiers, impacting the effectiveness of modifications.
Allow players to specialize in specific crafting disciplines, unlocking unique modifications and recipes.
High crafting skills could allow for experimentation and improvisation, enabling players to create unique modifications or even entirely new items not found in blueprints.
#### Modification Rarity

- **Common:** These modifications are relatively easy to find or craft and provide basic bonuses.
- **Rare:** These modifications are more difficult to find or require high-level crafting skills and rare materials. They provide significant bonuses and unique effects.
### Item Degradation

- Items degrade over time with use, reducing their effectiveness.
- Players can repair their equipment using the Repair skill and appropriate materials.
- Different levels of degradation can be implemented, with heavily degraded items having significantly reduced stats and requiring more resources to repair.

## Part 6:  Settlement Building System

### Building Types

10 different building types are available, each with unique functions and upgrade paths:
- **Living Quarters:** Provide housing for the settlement's population. Upgrading increases capacity and living conditions.
- **Water Purification Plant** Provides clean water for the settlement. Upgrading increases water production and improves water quality.
- **Power Generator** Generates power for the settlement. Upgrading increases power output and allows for powering more advanced structures.
- **Clinic** Provides medical care for the settlement's population. Upgrading improves healing effectiveness and unlocks advanced medical procedures.
- **Research Lab** Allows for researching new technologies and blueprints. Upgrading unlocks more advanced research projects and attracts skilled scientists.
- **Workshop:** Provides a central location for crafting and modifying weapons, armor, and tools. Upgrading unlocks more advanced crafting options and improves crafting efficiency.
- **Trading Post** Facilitates trade with other settlements and traveling merchants. Upgrading attracts more traders and improves trade deals.
- **Defense Structures** Walls, turrets, and other defensive structures protect the settlement from attacks. Upgrading increases their defensive capabilities and offensive power.
- **Player house**

- Building costs and construction times scale with complexity and upgrade level.
- Buildings interact with each other to create a dynamic settlement system.
- Expand on building descriptions to highlight synergistic effects between specific structures.
- High-level buildings could offer unique benefits and interactions.
### Building Requirements

Each building type has specific requirements for construction:

- **Resource costs:** The amount and type of resources needed to build the structure.
- **Construction time:** The time it takes to complete the construction of the building.
- **Prerequisite buildings or technologies:** Some buildings might require other structures or technologies to be built first.
### Voting System

- Each player gets one vote per day for the building they want to prioritize.
- Players can campaign and debate to influence others' votes.
- The building with the most votes receives a 20% construction progress bonus.
### Building Upgrades

- Each building has 3 upgrade levels, unlocking new features and increasing efficiency.
- Upgrades require specific resources and may depend on research progress in the Research Lab.
### Settlement Management

- Players manage resources, population, happiness, and defenses within the settlement.
- This involves making strategic decisions about resource allocation, assigning jobs to NPCs, and ensuring the overall well-being and safety of the settlement.
- Defensive structures provide both passive and active defense during attacks, with higher levels offering greater protection and offensive capabilities.
- Introduce random events specific to the settlement, requiring players to collaborate and make decisions to resolve them.

#### Settlement Growth

Settlements can grow and expand by:

- **Increasing population:** Building more Living Quarters and improving happiness levels attracts more people to the settlement.
- **Upgrading buildings:** Upgrading existing buildings improves their efficiency and unlocks new features.
- **Researching new technologies:** The Research Lab allows players to research new technologies that can improve various aspects of the settlement.

#### Settlement Defense Strategies

Players can use various strategies to defend their settlement:

- **Defensive structures:** Building walls, turrets, and other defensive structures to deter and repel attackers.
- **NPC guards:** Assigning NPCs to guard duty, providing additional firepower and manpower during attacks.
- **Player participation:** Players can actively participate in combat during attacks, using their skills and equipment to defend the settlement alongside NPCs.

### Player housing

The player housing system allows players to own and personalize their own space within settlement. This system adds another layer of depth and immersion to the game, fostering a stronger connection between players and the communities they contribute to.

#### Acquiring Housing

- Players can purchase plots of land within settlements using bottle caps or other in-game currency.
- The size and location of the plot may influence the cost.
- Certain reputation levels with the settlement or specific factions might be required to access certain plots.

#### Building and Customization

- Players can construct and customize their houses using a variety of materials and furniture items.
- Building materials can be acquired through exploration, crafting, or purchasing from vendors.
- Furniture and decorations can be crafted, found as loot, or purchased from vendors.
- Players can personalize their houses with different themes, layouts, and functionalities.

#### House Functionality

- Houses can provide storage space for items and resources.
- Players can display trophies and achievements within their houses.
- Houses can serve as a social hub for inviting friends and group members.
- Certain upgrades might allow for crafting stations, resource production, or even NPC vendors within the house.
#### Benefits of Player Housing
- **Increased Immersion:** Provides players with a personal space to call their own, enhancing their connection to the game world and community.
- **Customization and Creativity:** Allows players to express their creativity and personalize their houses to reflect their individual style and preferences.
- **Utility and Functionality:** Offers practical benefits like storage space, crafting stations, and social gathering areas.
- **Community Building:** Encourages interaction and collaboration between players as they visit each other's houses and share resources or ideas.
## Part 7:  Economy and Trade System

### Currency

- Bottle caps are the primary currency, with rarer items like pre-war money having higher value.
- Pre-war money can be used for special purchases or as a status symbol.
- Bartering skill and charisma can influence trade prices by up to 20%.
### Player Trading

- Players can set up personal shops in the settlement marketplace to sell items for bottle caps or barter with other players.
- Direct trading between players allows for negotiation and customized deals.
### Shop

- The settlement shop offers only basic items required for starting out and establishing basic farming operations.
- Advanced items can only be acquired through crafting or trading.

### Bottle Cap Acquisition

Players can acquire bottle caps through various means:
- **Looting:** Bottle caps can be found while exploring the wasteland.
- **Completing quests:** Quests often reward players with bottle caps.
- **Trading:** Players can trade items with NPCs or other players for bottle caps.
- **Selling items:** Players can sell items they don't need at shops or through their own personal shops.
### Economic Fluctuations
- The game could feature a dynamic economy where prices and resource availability fluctuate based on player actions and market conditions.

## Part 8: Additional Mechanics

### Quests

- Over 30 quests are available, ranging from simple fetch quests to complex story-driven missions.

- Quests provide a variety of challenges and objectives, keeping gameplay engaging and motivating players to explore the world.

- Quest rewards include experience, bottle caps, unique items, and reputation gains.

#### Categories
- **Main story quests:** These quests advance the main narrative and reveal the secrets of the game world.
- **Side quests:** These quests provide additional challenges, rewards, and opportunities to explore the world and interact with NPCs.
- **Faction quests:** These quests are specific to individual factions and can improve the player's reputation with that faction.
- **Repeatable quests:** These quests can be completed multiple times, often providing resources or experience points as rewards.

- Quests offer meaningful choices that can impact the game world and narrative, with some offering branching paths and different outcomes.

- Some quests could have branching paths that lead to drastically different outcomes, such as siding with different factions or influencing the fate of entire settlements.


#### Difficulty
- **Recommended Level:** Each quest has a recommended level, indicating the minimum level players should be to tackle the quest comfortably.
- **Enemy Strength:** The strength and number of enemies players will face during the quest.
- **Quest Objectives:** The complexity and challenge of the quest objectives.
### Events

- Over 20 random events can occur, ranging from finding a hidden cache to defending the settlement from raiders.
- Event outcomes can be influenced by player choices and actions.
- Events can have various impacts on gameplay, such as providing opportunities for acquiring rare resources or items, introducing new challenges, affecting reputation, and triggering dynamic changes in the game world.

#### Event Triggers

- **Location:** Certain events might be specific to certain locations.
- **Time:** Some events might occur at specific times of day or during specific weather conditions.
- **Player actions:** Certain player actions might trigger specific events.
#### Event Consequences

- **Resource acquisition:** Events can provide opportunities to acquire rare resources or items.
- **New challenges:** Events can introduce new threats or challenges to the game world.
- **Reputation changes:** Events can affect the player's reputation with different factions.
- **Dynamic changes:** Events can trigger dynamic changes in the game world.
### Social Interaction

- Players can chat publicly or privately, form groups, and engage in roleplay.
- Group activities can provide bonuses to experience gain and resource gathering.
- Implement a mentorship system where experienced players can guide newer players.

## Part 9: User Interface and Controls

#### Overview
##### Interface Design
- Text-based interface with menus, descriptions, and interactive commands.
- The interface is designed to be clear, concise, and easy to navigate using text commands.
- The UI could be designed to resemble a Pip-Boy from the Fallout universe, displaying information in a retro-futuristic style.
##### Navigation and Menus
- Players navigate through menus using simple text commands and keywords.
- The command system should be intuitive and recognize synonyms and abbreviations to make navigation efficient and user-friendly.
- Context-sensitive commands are available within each menu for specific interactions.
##### Controls and Input
- Players primarily use text commands and keywords to interact with the game world.
- The game should recognize a variety of synonyms and abbreviations for commands.
- Implement a context-sensitive command system where available commands change depending on the player's current situation and surroundings.
#### Game interfaces

##### Player creation interface
- displays step to create new player
##### Player level up interface
- displays available skill points and attribute points
#### Player house interface
- displays player house
- displays player archivements and trophies
- displays in-house storage
- display actions and commands
##### Character information interface
- display current stats and attributes
- display current positive and negative effects
##### Player inventory interface
- displays items with description
- displays equippied items
- displays usable items
- displays quest items
##### Feedback and Information Interface
- Detailed descriptions provide feedback on actions and immerse players in the world.
- Descriptions should be vivid and engaging, painting a picture of the environment, characters, and events in the player's mind.
- The UI displays information about character stats, inventory, crafting, settlement status, and other relevant game elements.
- The information should be presented clearly and concisely.
###### Error Handling and Feedback
- The UI provides clear and informative feedback to players when actions fail or encounter issues.
- This includes specific error messages, visual or audio cues, and suggestions for alternative actions.
##### Chat 
- **Channels:** Public channels for general chat, faction chat, and group chat.
- **Private messages:** Players can send private messages to individual players.
- **Emotes:** Players can use emotes to express emotions and actions in chat.
##### Group
- **Form groups:** Create and manage groups with other players.
- **Invite players:** Invite other players to join their group.
- **Assign roles:** Assign roles within the group, such as leader, scout, or medic.
- **Coordinate activities:** Share quest objectives, track group resources, and plan strategies.
##### Trading
- **Set up personal shops:** Display items for sale and set prices.
- **Browse other players' shops:** Search for specific items or browse by category.
- **Engage in direct trades:** Trade items directly with other players, including barter options.
- **View item descriptions:** See detailed information about items before buying or trading.
##### World Map
- Displays the different routes and locations within the wasteland.
- Shows the player's current location and progress on each route.
- Allows players to select their destination and track their travel progress.
- Provides information about each location, such as resource availability, potential dangers, and available quests.
##### Crafting
- Displays available blueprints and modifications for each crafting station.
- Shows required materials and skill levels for crafting each item.
- Allows players to select modifications and customize their crafted items.
- Provides information about the effects and stats of each modification.
##### Settlement Management
- Provides an overview of the settlement's status, including resource levels, population, happiness, and defenses.
- Allows players to manage resources, assign jobs to NPCs, and prioritize building construction and upgrades.
- Displays information about each building's function, upgrade levels, and resource production.
- Shows the current voting status for prioritized building construction.

##### Settlement building interface
- displays detailed info about building
- display available commands and actions in this building (e.g. "Craft" for workbench)
##### Combat
- Shows character stats, AP, and available combat actions.
- Allows players to select targets, choose combat actions, and use items during combat.
- Provides feedback on combat actions, including damage dealt, critical hits, and status effects
## Part 10: Technical Specifications

### Overview

**Game Engine:** Node.js / TypeScript for server-side logic and Redis for data storage. This combination provides a robust and efficient platform for handling the game's backend processes and data management.

**Programming Language(s):** TypeScript for both server and client-side development. TypeScript offers strong typing and object-oriented features, ensuring code quality and maintainability.

**Art Style and Assets:** While primarily text-based, the game may incorporate stylized visuals for maps, character portraits, and key items. These visuals should be consistent with the game's post-apocalyptic setting and enhance the overall atmosphere and immersion.

**Sound Design and Music:** Atmospheric soundscapes and music enhance the game's immersion and setting. Sound effects and music should be carefully chosen to create a sense of danger and tension in the wasteland, while also reflecting the game's thematic inspiration from the Fallout universe.

**Network and Multiplayer:** WebSocket protocol enables real-time communication and interaction between players. This allows for smooth and responsive multiplayer gameplay, ensuring that players can interact with each other and the game world in real-time.

### Scalability and Performance Considerations

- Strategies for ensuring the game's scalability and performance with a large number of players and concurrent actions. This includes implementing efficient data structures, caching mechanisms, and load balancing techniques to distribute server load and prevent performance bottlenecks.
- Aim for high performance benchmarks that ensure a smooth and responsive gameplay experience even with a large number of players and complex interactions.
- **Performance Optimization:** Outline the strategies used to optimize game performance and ensure scalability with a large player base.
### Data Persistence

- Game data is persisted using a combination of Redis for real-time data and a persistent database (e.g., MongoDB) for long-term storage. This ensures that player progress and game world data are saved and can be accessed even after players log out or servers restart.
- **Data Backup and Recovery:** Explain the procedures for data backup and recovery in case of server failure or data loss.
### Security Measures

- Data validation, encryption, and user authentication protocols are implemented to protect game data and prevent cheating or malicious activity.
- **Anti-Cheat Measures:** Describe the specific measures implemented to prevent cheating and maintain fair play in the game.

## Part 11: Development Roadmap

**Phase 1: Core Gameplay Development (Estimated Time: 3-4 months)**

- **Character Creation and Development:** Implement the S.P.E.C.I.A.L. system, skills, perks, and traits.

- **Exploration:** Develop the world map and initial set of locations for each route, including resource gathering mechanics.

- **Crafting:** Implement crafting stations, blueprints, and modification systems for weapons, armor, and other items.

- **Settlement Building:** Design and implement basic settlement building mechanics, including building types, resource costs, construction times, and the voting system.

- **Combat:** Develop the turn-based combat system, including enemy types, combat actions, and how character stats and skills influence combat outcomes.

- **Social Interaction:** Implement basic chat and group formation functionalities.

- **Internal Testing and Feedback:** Conduct thorough internal testing of the core gameplay loop and gather feedback from the development team and early adopters.

**Phase 2: Content Expansion and Refinement (Estimated Time: 4-6 months)**

- **Expand the World:** Add more locations to each route, creating diverse environments and challenges.

- **Quests and Events:** Develop a variety of quests, including main story quests, side quests, faction quests, and repeatable quests. Implement random events that occur during exploration and within settlements.

- **Lore and Story:** Integrate lore elements into the game world through environmental storytelling, quest dialogues, and NPC interactions.

- **Dynamic World Events:** Introduce large-scale events that impact the entire game world, requiring players to collaborate and adapt.

- **Player-Driven Economy:** Develop a dynamic economy where prices and resource availability fluctuate based on player actions and market conditions.

- **Refinement and Balancing:** Refine existing mechanics based on player feedback gathered from playtesting the prototype. This includes balancing combat, crafting, settlement building, and other gameplay elements

- **Seasonal Content and Challenges:** Implement a system for introducing limited-time events, special rewards, and unique challenges that change with the seasons.


**Phase 3: Advanced Features and Polishing (Estimated Time: 3-4 months)**

- **Guilds and Factions:** Implement guild and faction systems, allowing players to form groups with shared goals and compete for influence in the wasteland.
- **PvP and Cooperative Gameplay:** Introduce optional PvP elements and expanded cooperative gameplay features, such as raids and group challenges.
- **Deeper Settlement Management:** Expand settlement management mechanics to include resource production, population growth, and more complex defense systems.
- **Polishing and Bug Fixing:** Address any remaining bugs and fine-tune game mechanics to ensure a smooth and enjoyable gameplay experience.
- **Marketing and Launch:** Prepare marketing materials, such as trailers, screenshots, and website content. Launch the game on the chosen platforms and implement monetization strategies.

## Part 12: Marketing and Publishing

### Target Market

- **Primary Target:** Fans of Fallout, post-apocalyptic settings, and text-based MMORPGs.
- **Secondary Target:** MMORPG players who enjoy collaborative gameplay, strategy elements, and deep character customization.

### Marketing Strategy

#### Community Building
- Establish a strong online presence through social media platforms, forums, and a dedicated website.
- Create engaging content, such as developer blogs, lore snippets, and behind-the-scenes glimpses into the development process.
- Actively interact with the community, respond to feedback, and foster a sense of belonging and excitement.
#### Influencer Marketing
- Partner with influencers and content creators who cater to the target audience.
- Provide early access to the game and collaborate on promotional content, such as gameplay videos and reviews.
#### Targeted Advertising
- Utilize targeted advertising on social media platforms and gaming websites to reach potential players who align with the game's target demographic.
#### Content Marketing
- Create high-quality content, such as blog posts, articles, and infographics, that provide value to the target audience and promote the game's unique features and setting.
#### Public Relations
- Reach out to gaming publications and journalists to secure coverage and reviews of the game.
- Participate in gaming conventions and events to showcase the game and generate interest.

### Publishing Plan

- **Self-Publishing:** Self-publish the game on web browser and Telegram Mini Apps platforms. This allows for greater control over the publishing process, direct interaction with the player community, and flexibility in updating and expanding the game.
- **Platform Partnerships:** Explore potential partnerships with other gaming platforms to expand the game's reach and audience.

### Localization

- Consider localizing the game into different languages to expand its reach and cater to players from different regions.
- This may involve translating game text, interface elements, and marketing materials.

### Community Management
- Establish clear community guidelines and rules to foster a positive and inclusive environment for all players.
- Actively moderate forums and chat channels to address player concerns, resolve conflicts, and ensure a safe and enjoyable experience for everyone.
- Regularly collect and respond to player feedback to improve the game and address community concerns.

## Part 13: Conclusion

Wasteland Chronicles is an ambitious project that aims to create a unique and engaging text-based MMORPG experience. By combining elements of exploration, crafting, settlement building, combat, and social interaction, the game offers a rich and immersive world for players to explore and conquer. The detailed design document outlined in this GDD provides a comprehensive roadmap for the development team, ensuring a clear vision and direction for the project. With careful planning, execution, and ongoing community engagement, Wasteland Chronicles has the potential to become a successful and beloved online game that captures the hearts and imaginations of players who seek adventure and camaraderie in a post-apocalyptic world.