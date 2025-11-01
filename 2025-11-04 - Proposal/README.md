# Project Title: Our Project Name

Edit this file to contain your project proposal. Use proper markdown formatting. Your proposal will be reviewed to determine whether it is "enough work" or "too much work" for the scope of the course. 

It should describe the following information, and be approximately 2-3 pages in length:

- Game name / genre / overall theme / main gameplay style
- Examples of gameplay scenarios involving each of the game mechanics described below
- A list of "extra" features of the game which have not yet been completed in assignments 

## Introduction
[Game Name] will be a platformer with two-dimensional, side-scroller graphics style. Players of [Game Name] will explore multiple distinctly-styled stages where they will fight enemies using a customizable wand. Their goal is to bring order to chaos by defeating a boss on each stage; the catch is, each boss is a different data structure encountered in Computer Science that must be properly interacted with in order to progress to the next stage. While being a standalone game in its own right, [Game Name] can also serve as a sort of learning tool for some simple CS data structures (think stacks, queues, etc.) by way of defeating the bosses and hence progressing through the game.

[Game Name] will facilitate players' traversal of each level by giving them the ability to upgrade their wands by essentially building them up from a basic projectile weapon. Players will be able to obtain upgrades such as increased bullet speed, enemy lock-on, wall penetration and more. Each upgrade can stack and ultimately allow players to shape their wand in the way that fulfills their preferred play style. Upgrades can be obtained **throughout each level through a randomized list (discuss with group)** .

## Gameplay and Mechanics
[Game Name] will fully satisfy the required project mechanics:

- **Collisions**: Players will traverse a 2D, sidescroller environment where their character must follow the level's environment design (cannot go through walls/floors). All interactable (i.e. not decorative) entities will have bounding boxes used by AABB collision detection in order to resolve situations like bullet hit registration.

- **Movement**: In addition to regular WASD movement, players will be able to **(discuss with group)**

- **Bullets/Weapons**: Where the wand is highly customizable, it alone will satisfy the requirement of 3+ unique weapons. **(Discuss how to implement rest of this mechanic)**

- **NPCS**: Players will face numerous unique enemies on their journey, each with their own attack style. While some are static, turret-like enemies, others actively patrol the stage, attacking when the player is in view.

- **Hitpoints/I-Frames**: Both the player and NPCs will have hitpoints and i-frames. Players will be able to see both their own hitpoints and their enemy's. When the player's hitpoints reach zero, they will have to restart the current stage. When an enemy's hitpoints reach zero, they will be permanently removed from the current instance of the stage.

- **Objects/Inventory**: Players will be able to obtain item drops (whether from the environment or as drops from enemies) that boost their character in different ways such as health regeneration, movement speed buff, damage buff, anti-gravity, etc. These items will be visible in the player UI and selectable/usable via hotkeys.

- **Ray Casting**: NPC vision will use ray casting in order to detect and attack the player.

- **Gravity/Acceleration**: The player character, all NPCs, and possibly some special terrain will be affected by gravity (unless afflicted with a status affect/buff).

- **Camera/World View**: In addition to the player character's limited world view, players will be able to see a map with the full stage layout and their location within.

- **Audio**: [Game Name] will *possibly* feature original music mixed with pre-made music and sounds that play when their respective entity is interacted with in numerous ways (health loss, death, etc.).

- **Assets**: [Game Name] will feature unique assets not previously provided in class.

- **Options**: Players will be able to adjust game settings such as audio, difficulty level, and keybinds.

- **Game Progression**: Overall game progression will be locked behind the completion of each stage. The player will be able to save their current overall game progression (NOT individual level progression).

- **Status Effects**: Numerous status effects will afflict players and NPCs alike through the means of spells/pickups. This includes effects like anti-gravity, burning (damage-over-time), and movement speed.

- **User Interface/HUD**: Players will be able to see a UI that tracks important information like pickups, health, current status afflictions w/ timers, etc.

- **Moving Tiles**: Players will interact with moving pieces of environment, be it for puzzle completion or stage traversal.

- **Shaders**: Different status effects will apply unique shaders to entities in order to visually signify that the entity is afflicted with the effect.

- **Parallax**: The background of each stage will be layered in order to create a more deep, interesting environment.

- **Lighting**: Some spells/environmental entities will illuminate the environment around them.

- **Pathfinding**: Aggressive NPCs will be implemented with path-finding in order to shoot/get to the player. This can also possibly be used as a wand property.

- **Extra**: **(Discuss)**
