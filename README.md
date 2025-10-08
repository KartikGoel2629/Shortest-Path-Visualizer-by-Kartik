# Shortest Path Visualizer

## About
This project provides a graphical simulation of shortest-path algorithms on a grid. You can interactively place obstacles, choose start and end nodes, and see how various algorithms explore the grid and find paths.It’s built in Python using pygame for rendering and interaction.

## Features — Supported Algorithms

The visualizer currently supports:

-Breadth-First Search (BFS) — guarantees shortest path in unweighted grids
-Depth-First Search (DFS) — does not guarantee shortest path
-Dijkstra’s Algorithm — for weighted or unweighted graphs (guarantees shortest path)
-A* (A-star) — heuristic-driven search, typically faster, still finds shortest path

### Other features:

-Interactive grid: click to create obstacles, set start & end
-Clear / reset grid
-Visual step-by-step exploration
-Speed control (if implemented)
-Real-time feedback, coloring of visited nodes & final path

## How It Works

Grid Representation
The map is represented as a 2D grid (rows × columns). Each cell is a node (or tile) that may be open or an obstacle.
 
Neighbors & Edges
From each non-obstacle tile, edges connect to its neighboring (up/down/left/right or optionally diagonals) tiles.

Algorithm Execution

BFS / DFS — use queue or stack to explore neighbors

Dijkstra / A* — maintain a priority queue, distances, parent pointers, and a heuristic (for A*)

Visualization Steps

Mark nodes as visited (change color)

When the target node is reached, backtrack via parent links to draw the final path

Optionally show “frontier” nodes, cost labels, or distances

User Interaction

Left-click on a cell → toggle obstacle

Right-click → place start or end node

Buttons / UI controls to start algorithm, reset, clear, etc.

Optionally, allow speed control or pause / step mode

### Screenshot
![image](https://github.com/user-attachments/assets/400716ae-676c-4cb4-ab57-6c5324f76ac5)
### Usage:
- `LEFT CLICK` to make obstacle
- `RIGHT CLICK` to create start and end node
- buttons for running algorithms
### To Run
install `pygame` pacakge
```
pip install pygame
```
then run the 'main.py' file
```
python main.py
```
