
# Console Game - Food Eater

This is a simple console-based game called "Food Eater," where the player controls a character represented by different states and tries to eat randomly appearing food items. The goal is to eat as much food as possible by moving the player around the console window. The game includes various features, such as random food generation, different player states, and player movement controls.

## Table of Contents
- [Challenge-project-Create-methods-in-CSharp](#challenge-project-create-methods-in-csharp)
- [Console Game - Food Eater](#console-game---food-eater)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Getting Started](#getting-started)
    - [Requirements](#requirements)
    - [Installation](#installation)
  - [How to Play](#how-to-play)
    - [Controls](#controls)
    - [Player States](#player-states)
    - [Food](#food)
  - [Game Mechanics](#game-mechanics)
  - [Documentation](#documentation)
  - [License](#license)

## Introduction

Food Eater is a simple game developed in C# that runs in the console window. The player can control the character using arrow keys and try to eat food items that randomly appear on the screen. The game provides a fun and interactive experience within the console environment.

## Getting Started

### Requirements

To play and run the game, you will need the following:

- .NET Framework installed on your system.
- A console window on your operating system (Windows, macOS, or Linux).

### Installation

1. Clone this repository to your local machine.
2. Navigate to the project directory using the command prompt or terminal.
3. Build the project using the .NET CLI:
   ```
   dotnet build
   ```
4. Run the game using the .NET CLI:
   ```
   dotnet run
   ```
5. The game will start in the console window, and you can begin playing.

## How to Play



### Controls

- Use the **arrow keys** (Up, Down, Left, Right) to move the player character.
- Press the **Escape** key to exit the game.

### Player States

The player character can be in three different states:

1. **Happy:** Represented by the character `('-')`. The default state of the player when the game starts.
2. **Excited:** Represented by the character `('^-^')`. When the player eats certain food, it becomes faster and changes to this state.
3. **Sick:** Represented by the character `('(X_X)')`. If the player eats specific food, it becomes sick and freezes for a short time.

### Food

- The game displays various food items represented by strings such as `@@@@@`, `$$$$$`, and `#####`.
- The player needs to move over the food items to eat them and change their appearance.

## Game Mechanics

- The game starts with the player character in its default "Happy" state.
- The food items appear at random positions on the console window.
- As the player character moves over the food items, it consumes them.
- Consuming different types of food changes the appearance and behavior of the player character.
- Eating specific food items can make the player character faster or make it freeze temporarily.
- The game continues until the player decides to exit or the console window is resized.

## Documentation

This project's code is documented using inline comments, which provide a detailed explanation of the code's functionality and logic. The following are the main functions and their purposes:

1. `TerminalResized()`: Checks if the console window has been resized.
2. `ShowFood()`: Displays random food at a random location on the console.
3. `GotFood()`: Checks if the player character has eaten the food.
4. `PlayerIsSick()`: Checks if the player character is in a sick state.
5. `PlayerIsFaster()`: Checks if the player character is in an excited (faster) state.
6. `ChangePlayer()`: Updates the player character appearance based on the consumed food.
7. `FreezePlayer()`: Temporarily stops the player character from moving.
8. `Move(int speed, bool otherKeysExit)`: Reads directional input from the console and moves the player character.
9. `InitializeGame()`: Clears the console, displays the food, and places the player character at the starting position.



## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
