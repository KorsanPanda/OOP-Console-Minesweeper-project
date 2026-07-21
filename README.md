# 💣 OOP Console Minesweeper Project

![Language](https://img.shields.io/badge/Language-C++-blue.svg)
![Paradigm](https://img.shields.io/badge/Paradigm-OOP-green.svg)
![Interface](https://img.shields.io/badge/Interface-Console-orange.svg)
![Build](https://img.shields.io/badge/Build-Makefile-purple.svg)

A C++ console-based implementation of the classic **Minesweeper** game, designed using core **Object-Oriented Programming (OOP)** principles. It features custom grid sizes, dynamic mine placement, coordinate-based tile uncovering, and flag placement.

---

## 📌 Project Overview

This project refactors the traditional Minesweeper mechanics into a modular, object-oriented C++ application. The game handles grid generation, neighbor mine calculations, path uncovering (including zero-mine chain reveals), and state tracking directly within the terminal interface.

### Key Features
* **Object-Oriented Design:** Clear separation of concerns utilizing classes for the board, tiles, and game logic management.
* **Dynamic Grid & Mine Allocation:** Configurable board dimensions and mine counts.
* **Recursive Zero-Reveal:** Automatically unveils adjacent safe tiles when a tile with zero adjacent mines is cleared.
* **Interactive Command System:** Input coordinates to reveal tiles or toggle flags safely.
* **Game State Tracking:** Real-time feedback for wins, losses, remaining flags, and elapsed game state.

---

## 🚀 Getting Started

### Prerequisites
* A C++ compiler supporting C++11 or higher (e.g., `g++` via MinGW on Windows or native GCC/Clang on Linux/macOS)
* `make` utility (optional, if Makefile is provided)

### Building and Running

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/USERNAME/OOP-Console-Minesweeper-project.git](https://github.com/USERNAME/OOP-Console-Minesweeper-project.git)
   cd OOP-Console-Minesweeper-project
   ```

2. **Compile the project:**
   * Using Makefile:
     ```bash
     make
     ```
   * Or using G++ directly:
     ```bash
     g++ -std=c++11 src/*.cpp -Iinclude -o bin/Minesweeper
     ```

3. **Run the executable:**
   * **Windows:**
     ```cmd
     .\bin\Minesweeper.exe
     ```
   * **Linux / macOS:**
     ```bash
     ./bin/Minesweeper
     ```

---

## 🎮 How to Play

1. Launch the game and select your desired difficulty or grid size.
2. Enter coordinates along with an action:
   * **Reveal tile:** Enter row and column numbers (e.g., `r 3 4` or `3 4`).
   * **Flag / Unflag tile:** Toggle a flag on suspected mine locations (e.g., `f 3 4`).
3. Clear all safe tiles without detonating a mine to win the game!

---

## 📁 Directory Structure

```text
OOP-Console-Minesweeper-project/
├── bin/
│   └── Minesweeper.exe      # Generated executable file
├── include/
│   ├── Board.h              # Board class definition & grid management
│   ├── Tile.h               # Tile class definition & state attributes
│   └── Game.h               # Main game loop & interaction handling
├── src/
│   ├── Board.cpp            # Grid generation & recursive reveal logic
│   ├── Tile.cpp             # Tile behavior implementation
│   ├── Game.cpp             # Input parsing & game state checks
│   └── Main.cpp             # Program entry point
└── Makefile                 # Build script for compilation
```
