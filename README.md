# 💣 OOP Console Minesweeper Project

![Language](https://img.shields.io/badge/Language-C%2B%2B-blue.svg)
![Paradigm](https://img.shields.io/badge/Paradigm-OOP-green.svg)
![Interface](https://img.shields.io/badge/Interface-Console-orange.svg)
![Compiler](https://img.shields.io/badge/Compiler-GCC%20%2F%20G%2B%2B-purple.svg)

A C++ console-based implementation of the classic **Minesweeper** game, designed using core **Object-Oriented Programming (OOP)** principles including class inheritance, polymorphism, virtual functions, and recursive path-uncovering logic.

---

## 📌 Project Overview

This project implements the traditional Minesweeper mechanics inside a clean, object-oriented single-file structure. It features dynamic grid generation, random mine scattering, adjacent mine counts, exception handling for invalid user inputs, and recursive clearing of blank tiles.

### Key Features
* **Object-Oriented Architecture:**
  * `Oyun`: Abstract base class defining virtual game interface functions (`tahtaGoster`, `hamleYap`, `kazandiMi`).
  * `Hucre`: Encapsulates tile states (`mayinMi`, `acildiMi`, `komsuMayinlar`).
  * `MayinTarlasi`: Derived class handling game board generation, vector grids, and game state management.
* **Selectable Difficulty Levels:**
  * **1 - Easy:** $5 \times 5$ Grid, 5 Mines
  * **2 - Medium:** $6 \times 6$ Grid, 8 Mines
  * **3 - Hard:** $7 \times 7$ Grid, 10 Mines
* **Recursive Zero-Reveal Algorithm:** Automatically unveils neighboring tiles whenever a tile with 0 adjacent mines is selected.
* **Robust Input Handling:** Uses `try-catch` blocks to catch out-of-bounds coordinate entries (`std::out_of_range`) without crashing the application.

---

## 🎮 How to Play

1. Run the application and enter your preferred difficulty level (`1`, `2`, or `3`).
2. Input target coordinates step-by-step:
   * **Row number:** `0` to `N-1`
   * **Column number:** `0` to `N-1`
3. Uncover all non-mined tiles (`#` hidden $\rightarrow$ numbers revealed) to win the game!
4. Detonating a mine (`*`) triggers an immediate **GAME OVER**.

---

## 🚀 Getting Started

### Prerequisites
* A C++ compiler supporting C++11 or higher (e.g., `g++` via MinGW on Windows or native GCC/Clang on Linux/macOS).

### Compiling and Running

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/KorsanPanda/OOP-Console-Minesweeper-project.git](https://github.com/KorsanPanda/OOP-Console-Minesweeper-project.git)
   cd OOP-Console-Minesweeper-project
   ```

2. **Compile the source file:**
   ```bash
   g++ MayinTarlasi -o MayinTarlasi.exe
   ```

3. **Run the executable:**
   * **Windows:**
     ```cmd
     .\MayinTarlasi.exe
     ```
   * **Linux / macOS:**
     ```bash
     ./MayinTarlasi.exe
     ```

---

## 📁 Directory Structure

```text
korsanpanda-oop-console-minesweeper-project/
├── MayinTarlasi          # Main C++ source code file (OOP classes & game loop)
└── README.md             # Project documentation
```
