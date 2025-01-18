# text-based-forest-game

---
## Mystery of the Forgotten Forest

A text-based adventure game written in C++, where the player explores a mysterious forest, makes choices, and attempts to escape while managing health and inventory.

## Overview

"Mystery of the Forgotten Forest" is a simple text-based adventure game written in C++. In this game, the player wakes up in a mysterious, foggy forest with no memory of how they got there. The goal is to escape the forest by making choices at different points in the game. Along the way, the player encounters challenges, discovers items, and manages their health.

---
## Game Features

*   **Text-Based Interaction:** The game is entirely driven by text input and output, allowing the player to make choices by typing commands.
*   **Object-Oriented Design:** The game utilizes a `Player` class to represent the player character, encapsulating the player's name, health, and inventory.
*   **Decision-Driven Gameplay:** The game progresses based on player choices at different points of the game, leading to different game events and outcomes.
*   **Inventory Management:** The player can collect items during the game (e.g., "Magic Potion", "Forest Key"), which can be viewed at any time using the `check` command.
*   **Health Management:** The player's health is tracked, and it can be reduced due to encounters with creatures in the game. The game ends when the health drops to zero.
*   **Multiple Endings:** The game can end in two ways:
    *   **Successful Escape:** By obtaining a specific item (Forest Key) and using it to escape through a gate.
    *   **Game Over:** When the player's health reaches zero.
*   **Basic Error Handling:** Handles invalid inputs by looping back to the user and requesting proper input.
*   **Linear Gameplay:** The gameplay is more linear and only depends on user choices.

---
## Game Flow

1.  **Introduction:** The game starts with a welcome message, setting up the game's story and objective.
2.  **Forest Path:** The player stands at a fork in the path and must choose to go left, right, explore the clearing, or escape.
3.  **Encounters & Exploration:** Depending on the player's choices, they might:
    *   **Encounter a Creature:** They must decide whether to fight, run, or check their inventory. If they choose to fight, they will lose health points.
    *   **Find a Treasure:** They can choose to open a treasure chest and find an item, or leave the treasure behind.
    *   **Explore the Clearing:** They can choose to inspect a mysterious stone, where a riddle has to be solved or just leave the clearing.
4.   **Solving a Puzzle:** If the player chooses to inspect the stone in the clearing, they must solve a riddle to continue in the game.
5.   **Escaping:** If the player has solved the riddle and has the "Forest Key", they can escape the forest. Otherwise, they must acquire the "Forest Key" and then escape.
6.  **Game End:** The game ends when the player either successfully escapes the forest or loses all health.

---
## Code Structure

*   **`main.cpp`:** Contains the main game logic.
*   **`Player` Class:** Represents the player character, their inventory, and health.
*   **`introduction()`:** Displays the game's introduction.
*   **`forestPath()`:** Manages navigation of the main path in the forest.
*   **`encounterCreature()`:** Handles creature encounters.
*   **`findTreasure()`:** Manages finding and interacting with treasures.
*   **`exploreClearing()`:** Manages exploring the clearing and interacting with a mysterious stone.
*    **`escapeForest()`:** Manages the event where the user tries to escape the forest.
*   **`solvePuzzle()`:** Provides the puzzle to be solved and manages the user choice.
*   **`displayHealth()`:** Displays health of the player.
*   **`checkGameOver()`:** Checks if health is zero and exits the game if the player lost all health.

---

