# Wall Is You

**Wall Is You** is a 2D puzzle‑adventure game set in a dynamic labyrinth full of enemies, treasures, and unique challenges. Unlike traditional games where you control a character, here the twist is that you play the labyrinth. Your main task is to rotate the walls to create a path through the maze, avoid enemies, and unlock hidden treasures. A personal touch added to the game is the Dragon Ball twist — featuring iconic characters like Goku and Gohan — which enriches the narrative and gameplay.

## Features

- **Customizable Gameplay**: Choose your character and explore various maps.
- **Dynamic Labyrinths**: Procedurally generated or pre-designed maps with unique challenges.
- **Interactive Elements**: Collect Dragon Balls, use Senzu Beans, and avoid enemies.
- **Special Game Mode : One Try Solve**: A unique challenge where you have only one chance to solve the labyrinth.
- **Map Editor**: Create and customize your own labyrinths.
- **Save and Load**: Save your progress and continue later.

## Installation
1. Install the required dependencies:
    ```bash
    python3 -m pip install --upgrade pip
    python3 -m pip install --upgrade Pillow pygame
    ```

2. Clone this repository:
    ```bash
    git clone https://github.com/your-repo/wall-is-you.git
    cd wall-is-you
    ```

## How to Play

1. Run the game:
   ```bash
   python3 wall_is_you.py
   ```
2. Use the menu to start a new game, load a saved game, or create a custom map.
## Rules & Mechanics

- You can only kill enemies that are at your level or below. By default, the character targets the enemy with the highest level, even if it’s too high, so you must block his route to force him towards an enemy he can defeat.
- When an enemy is defeated, your character levels up.
- Special Items:
  - **Senzu Bean**: If you pass by it, your character eats it automatically and levels up.
  - **Nimbus Cloud**: When encountered, it transports your character directly to an enemy at your level.
  - **Dragon Ball**: Place one on the map by right-clicking. When one is on the map, the character will prioritize moving towards it, if a valid path exists.
  
- **Space**: Moves the character once the path is set.
- **P**: Pause the game.
- **S**: Save the game.
- **R**: Restart the current map.

## Media

The game includes custom graphics and soundtracks:
- **Background Images**: Found in `Media/background_images/`.
- **Characters**: Found in `Media/characters/`.
- **Music**: Found in `Media/Music/`.

## Map Format

Maps are stored as text files in `Media/maps/`. Each map file defines the layout, player position, enemies, and items.

Example:
```
╔╦╦╦╦╗
╠╩╩╩╩╣
A 0 2
D 1 1 1
```