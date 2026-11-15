# 3D Survival Arena

A 3D survival game concept developed using C++ and Unreal Engine, focused on real-time player movement, combat, enemy behavior, collision detection, and game-state management.

## Overview

The game is designed around a survival arena where the player interacts with enemies in a real-time environment. The player can move around the arena, engage enemies, take damage, and continue playing while managing health and combat interactions.

The main focus of the project is understanding **C++ programming, Object-Oriented Programming, game logic, collision detection, enemy AI, and real-time game-state management**.

## Technologies Used

- C++
- Unreal Engine
- Object-Oriented Programming
- Game AI
- Collision Detection
- Game State Management

## Game Workflow

1. The game initializes the arena and game state.
2. The player is spawned into the game.
3. Enemy characters are created and placed in the arena.
4. The player moves around the environment and interacts with enemies.
5. Enemy AI controls enemy movement and behavior.
6. Collision detection identifies interactions between the player, enemies, and other game objects.
7. Combat interactions cause damage to the player or enemies.
8. Player health and game state are updated based on gameplay events.
9. The game continues until the required survival/game-ending condition is reached.

## Main Components

### Player

The player component manages:

- Player movement
- Health
- Combat actions
- Damage handling
- Interaction with enemies
- Player state

### Enemy

The enemy component manages:

- Enemy movement
- Enemy health
- Attack behavior
- Player detection
- Basic AI behavior
- Damage handling

### Game State

The game-state component manages information such as:

- Current gameplay state
- Player status
- Enemy status
- Score
- Game completion conditions

## Object-Oriented Design

C++ classes are used to separate different game entities and their responsibilities.

Example structure:

```text
Game
 |
 +-- Player
 |     +-- Movement
 |     +-- Health
 |     +-- Combat
 |
 +-- Enemy
 |     +-- AI
 |     +-- Movement
 |     +-- Health
 |
 +-- Weapon
 |     +-- Damage
 |     +-- Attack
 |
 +-- Game State
       +-- Score
       +-- Game Status
```

This separation helps keep the game logic organized and makes individual components easier to maintain.

## Enemy AI

The enemy AI controls how enemies behave during gameplay.

A basic behavior flow can be:

```text
Idle
  |
  v
Detect Player
  |
  v
Move Towards Player
  |
  v
Attack
  |
  v
Player Defeated?
  |
  +---- No ----> Continue
  |
  +---- Yes ---> Update Game State
```

The AI can use different states to determine what the enemy should do based on the current game situation.

## Collision Detection

Collision detection is used to identify interactions between game objects.

Examples include:

- Player colliding with an enemy
- Weapon/projectile hitting an enemy
- Enemy attacking the player
- Player interacting with objects in the arena

When a collision occurs, the appropriate game logic can be triggered, such as applying damage or updating the game state.

## Combat System

The combat system handles interactions between the player and enemies.

A typical combat flow is:

```text
Player Attack
     |
     v
Collision / Hit Detection
     |
     v
Identify Target
     |
     v
Apply Damage
     |
     v
Check Health
     |
     +---- Health > 0 ---> Continue
     |
     +---- Health <= 0 --> Defeat / Remove Entity
```

## Game State Management

The game state keeps track of the current condition of the game.

Possible states include:

- Playing
- Player damaged
- Enemy defeated
- Game over
- Victory

Keeping game-state logic separate helps prevent different parts of the game from directly controlling the entire gameplay flow.

## Key Features

- 3D survival arena
- C++ based gameplay logic
- Player movement and combat
- Enemy AI behavior
- Collision detection
- Health and damage system
- Score management
- Game-state management
- Object-oriented game architecture

## Learning Objectives

This project focuses on understanding:

- C++ classes and objects
- Inheritance and polymorphism
- Encapsulation
- Pointers and object references
- Game loops and real-time processing
- Collision detection
- Basic AI behavior
- Memory and object management
- Event-driven game logic
- Game-state management

## Future Enhancements

- Multiple enemy types
- Advanced enemy AI
- Weapon and inventory systems
- Different arena levels
- Power-ups
- Improved scoring system
- Save/load game state
- Multiplayer support

## Project Status

This repository contains the project documentation and design overview. The project can be extended with the complete Unreal Engine project and C++ source implementation.

## Author

**Bijivemula Susmitha**

C/C++ Developer | Software Engineer
