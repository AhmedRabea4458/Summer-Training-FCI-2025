<h1 align="center">Maze Adventure Game — Java OOP Project</h1>

<p align="center">
  A desktop maze game built with <strong>Java Swing</strong> applying core
  <strong>Object-Oriented Programming (OOP)</strong> concepts.<br/>
  Generate random mazes, move the player with smooth animation, solve the maze using DFS,
  and track time & score.
</p>

<p align="center">
  <!-- Shields -->
  <img src="https://img.shields.io/badge/Language-Java-ED8B00?logo=java&logoColor=white" />
  <img src="https://img.shields.io/badge/GUI-Java%20Swing-007396" />
  <img src="https://img.shields.io/badge/Paradigm-OOP-blueviolet" />
  <img src="https://img.shields.io/badge/Algorithm-DFS-green" />
  <img src="https://img.shields.io/badge/Project-Type%20Practical%20Exam-success" />
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-gameplay">Gameplay</a> •
  <a href="#-project-structure">Project Structure</a> •
  <a href="#-oop-concepts-used">OOP Concepts</a>
</p>

---

## 🎮 Features

- 🧩 **Random Maze Generation** using DFS (Depth First Search)
- 🎯 **Player Movement** with collision detection
- 🎞 **Smooth Animation** using Swing Timer
- 🧠 **Maze Solver** (DFS + Backtracking)
- ⏱ **Timer & Score System**
- 📊 **Difficulty Levels** (Easy / Medium / Hard)
- 🔊 **Sound Effects** (move, win, loss, error)
- 🪟 **Custom Dialogs** (Win / Lose / Confirm)
- 🧩 **Game State Management** (Start, Play, Solve, Finish)

---

## 🎮 Gameplay

- Use **Arrow Keys** to move the player
- Reach the **exit (goal)** to win
- Time decreases your score
- You can:
  - Start a new game
  - Change level
  - Let DFS solve the maze automatically

---

## 🧠 Algorithms Used

### 🔹 DFS (Depth First Search)

- Used in **Maze Generation**
- Used again in **Maze Solving**
- Implemented using **Stack (Iterative DFS)**

---

## 🧩 OOP Concepts Used

- **Encapsulation**
  - Player position, movement, score, timer
- **Abstraction**
  - Maze generation & solving logic separated
- **Inheritance**
  - Custom panels extend `JPanel`
- **Polymorphism**
  - KeyListener & event handling
- **Interfaces**
  - `GameOverListener` for loose coupling between components
- **Separation of Concerns**
  - UI, logic, and models are separated

---

## 🏗 Project Structure

```bash
Maze-Adventure/
├─ Main.java                # Entry point
├─ MazePanel.java           # Core game logic & rendering
├─ MazeGenerator.java       # Random maze generation (DFS)
├─ MazeSolver.java          # Maze solving (DFS)
├─ RightSidePanel.java      # Timer, score, level display
├─ navPanel.java            # Top navigation bar
├─ GameState.java           # Enum for game states
├─ GameOverListener.java    # Custom event interface
├─ SoundManager.java        # Sound handling
├─ Sound.java               # Sound enum
├─ CustomMessage.java       # Custom dialogs
├─ AppColors.java           # Centralized colors
├─ model/
│   ├─ Player.java          # Player logic & animation
│   └─ Level.java           # Level configuration
├─ resources/
│   ├─ sounds/
│   └─ icons/
└─ README.md
