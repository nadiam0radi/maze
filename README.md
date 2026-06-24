# Matter.js Maze Generator

A simple **random maze generator built with Matter.js** using a grid-based Depth First Search (DFS) algorithm. The maze is rendered in a physics-enabled canvas using Matter.js wireframe mode.

---

## 🚀 Features

- Random maze generation using **DFS backtracking**
- Grid-based structure (configurable size)
- Built with **Matter.js physics engine**
- Real-time rendering using Matter.js renderer
- Clean separation of:
  - grid tracking
  - wall tracking (horizontal + vertical)
  - maze generation logic

---

## 🧠 How It Works

The maze is generated using a **Depth First Search (recursive backtracking)** algorithm:

1. Start from a random cell
2. Mark it as visited
3. Randomly shuffle its neighbors (up, right, down, left)
4. For each valid unvisited neighbor:
   - Remove the wall between current cell and neighbor
   - Recursively continue from that neighbor

This creates a **perfect maze** (no loops, exactly one path between any two cells).

---

## 🏗️ Tech Stack

- JavaScript (ES6)
- Matter.js
- HTML Canvas (via Matter.Render)

---

## 📦 Project Structure

```text
.
├── index.html
├── script.js   # Main maze + physics logic
└── README.md
