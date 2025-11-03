# Project Title: Our Project Name

## Introduction
[Game Name] will be a platformer with two-dimensional, side-scroller graphics style. Players of [Game Name] will explore multiple distinctly-styled stages where they will fight enemies using a customizable wand. Their goal is to bring order to chaos by defeating a boss on each stage; the catch is, each boss is a different data structure encountered in Computer Science that must be properly interacted with in order to progress to the next stage. While being a standalone game in its own right, [Game Name] can also serve as a sort of learning tool for some simple CS data structures (think stacks, queues, etc.) by way of defeating the bosses and hence progressing through the game.

[Game Name] will facilitate players' traversal of each level by giving them the ability to upgrade their wands by essentially building them up from a basic projectile weapon. Players will be able to obtain upgrades such as increased bullet speed, enemy lock-on, wall penetration and more. Each upgrade can stack and ultimately allow players to shape their wand in the way that fulfills their preferred play style. Wand uppgrades are randomized and can be obtained either in static locations or as drops from enemies.

The overall theme of the game blends magic and computer science, creating a 
light-hearted but chaotic world where coding logic makes every spell. The game’s tone will be playful and slightly humorous, with logical puzzles and data-structure-inspired bosses that make the experience both fun and educational.

## Game Scenes
- [Game Name] will present the player with a main menu screen when initially launched. This screen will allow the user the choice of loading their game, change options, or launching the level editor.
- After opting to play in the main menu screen, players will be presented with the overworld map, where they can choose what level to play (depending on game progression).
- After selecting a level, the player will be placed within the main gameplay scene in which they will interact with the game's system.
- A separate level editor will be available aside from the main gameplay scene that allows the user to play with the game's systems.
- Upon death/loss, the player will be presented with a "Game Over" screen which will allow them to either quit or restart.

## Gameplay and Mechanics
[Game Name] will fully satisfy the required project mechanics:

- **Collisions**: Players will traverse a 2D, sidescroller environment where their character must follow the level's environment design (cannot go through walls/floors). All interactable (i.e. not decorative) entities will have bounding boxes used by AABB collision detection in order to resolve situations like bullet hit registration.

  ex. A spell cast at an enemy NPC will only damage them if their bounding boxes collide.

- **Movement**: In addition to regular WASD movement, players will be able to hover in the air for a fixed amount of time (if not on a supporting tile) and dash with i-frames. Both movement abilities will have a cooldown.

  ex. The player may hover over a small gap which would have caused damage to them.

- **Bullets/Weapons**: Where the wand is highly customizable, it alone will satisfy the requirement of 3+ unique weapons. The player will be able to carry multiple wands which they can swap using a hotkey during the game.

  ex. Wand 1 may be better than Wand 2 for dealing with certain situations.

- **NPCS**: Players will face numerous unique enemies on their journey, each with their own attack style. While some are static, turret-like enemies, others actively patrol the stage, attacking when the player is in view.

  ex. The player may encounter NPCs that shoot spells at them, reflect spells back at them, charge them with a melee attack, etc.

- **Hitpoints/I-Frames**: Both the player and NPCs will have hitpoints and i-frames. Players will be able to see both their own hitpoints and their enemy's. When the player's hitpoints reach zero, they will have to restart the current stage. When an enemy's hitpoints reach zero, they will be permanently removed from the current instance of the stage. Certain enemies can have alternate phases based on their hit points remaining.

- **Objects/Inventory**: Players will be able to obtain item drops (whether from the environment or as drops from enemies) that boost their character in different ways such as health regeneration, movement speed buff, damage buff, anti-gravity, etc. These items will be visible in the player UI and selectable/usable via hotkeys.

  ex. The player picks up a health potion off a dead enemy which restores their hit points if used.

- **Ray Casting**: NPC vision will use ray casting in order to detect and attack the player.

  ex. NPCs will spot the player if there isn't a solid object in the way.

- **Gravity/Acceleration**: The player character, all NPCs, and possibly some special terrain will be affected by gravity (unless afflicted with a status affect/buff).

  ex. Unless under the effect of anti-gravity, players and NPCs will logically fall downwards if there is no supporting tile underneath them.

- **Camera/World View**: In addition to the player character's limited world view, players will be able to see a map with the full stage layout and their location within.

  ex. A map that pops-up when a hotkey is pressed, and goes away when pressed again.

- **Audio**: [Game Name] will *possibly* feature original music mixed with pre-made music and sounds that play when their respective entity is interacted with in numerous ways (health loss, death, etc.).

  ex. The player hits an enemy NPC with a spell; the cast spell makes a noise and the NPC makes a noise as it takes damage.

- **Assets**: [Game Name] will feature unique assets not previously provided in class.

  ex. Pre-made asset packs available online in order to model terrain, NPCs, spells, etc.

- **Options**: Players will be able to adjust game settings such as audio, difficulty level, and keybinds.

- **Game Progression**: Overall game progression will be locked behind the completion of each stage. The player will be able to save their current overall game progression (NOT individual level progression).

- **Status Effects**: Numerous status effects will afflict players and NPCs alike through the means of spells/pickups. This includes effects like anti-gravity, burning (damage-over-time), and movement speed.

  ex. An enemy NPC hits the player with a fire spell; the player will be burning and take chip damage for a certain number of frames.

- **User Interface/HUD**: Players will be able to see a UI that tracks important information like pickups, health, current status afflictions w/ timers, etc.

  ex. A UI bar at the bottom/top of the screen that displays the current item(s) a player has with their respective sprite.

- **Moving Tiles**: Players will interact with moving pieces of environment, be it for puzzle completion or stage traversal.

  ex. A moving platform over perilous terrain that a player must time their jump to correctly land on and avoid damage.

- **Shaders**: Different status effects will apply unique shaders to entities in order to visually signify that the entity is afflicted with the effect.

  ex. An NPC under the burning effect will have a red hue.

- **Parallax**: The background of each stage will be layered in order to create a more deep, interesting environment.

  ex. Mountains, forest, underwater scenery, etc.

- **Lighting**: Some spells/environmental entities will illuminate the environment around them.

  ex. A fire spell saturates the colour of the pixels within a certain radius of it, creating a lighting effect.

- **Pathfinding**: Aggressive NPCs will be implemented with path-finding in order to shoot/get to the player.

  ex. An NPC will jump over a small wall in order to see the player.

- **Extra**: The game will feature a levelling system based on experience gained from enemies killed. Every level up will statically buff things such as the hover cooldown, dash cooldown, wand count, and base damage.

**Example Gameplay Scenario:**  
In the Recursion stage, every time the player damages the boss, it splits into smaller copies of itself. The only way to end the fight is to break the recursive loop by casting a “base case” spell. Failing to do so causes the boss to duplicate endlessly, eventually overwhelming the player in a chaotic loop of infinite enemies.

