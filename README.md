# Shortest Path Visualizer

##  About
- This project provides a **graphical simulation of shortest-path algorithms** on a grid.  
- You can **interactively place obstacles**, choose start and end nodes, and see how various algorithms explore the grid and find paths.  
- Built in **Python** using **Pygame** for rendering and interaction.  

---

##  Features — Supported Algorithms

###  Algorithms
- **Breadth-First Search (BFS)** — guarantees shortest path in unweighted grids  
- **Depth-First Search (DFS)** — does *not* guarantee shortest path  
- **Dijkstra’s Algorithm** — works for weighted or unweighted graphs (guarantees shortest path)  
- **A\*** (**A-Star**) — heuristic-driven search, typically faster, still finds shortest path  

###  Other Features
-  Interactive grid — click to create obstacles, set start & end points  
-  Clear / reset grid  
-  Visual step-by-step exploration  
-  Speed control *(if implemented)*  
-  Real-time feedback with coloring of visited nodes & final path  

---

##  How It Works

###  Grid Representation
- The map is represented as a **2D grid (rows × columns)**.  
- Each cell (tile) represents a **node** that may be open or an obstacle.  

###  Neighbors & Edges
- From each non-obstacle tile, edges connect to its **neighboring tiles** (up, down, left, right, or optionally diagonals).  

###  Algorithm Execution
- **BFS / DFS** — use a **queue or stack** to explore neighbors.  
- **Dijkstra / A\*** — maintain a **priority queue**, **distance map**, **parent pointers**, and (for A\*) a **heuristic function**.  

###  Visualization Steps
-  Mark nodes as *visited* by changing their color.  
-  When the target node is reached, **backtrack** through parent links to draw the final path.  
-  Optionally show “frontier” nodes, cost labels, or distances.  

###  User Interaction
- **Left-click** on a cell → toggle obstacle  
- **Right-click** → place **Start** or **End** node  
- Use **buttons / UI controls** to:
  - Start the algorithm  
  - Reset or clear the grid  
 


### Screenshot
![image](https://github.com/user-attachments/assets/400716ae-676c-4cb4-ab57-6c5324f76ac5)

### To Run
install `pygame` pacakge
```
pip install pygame
```
then run the 'main.py' file
```
python main.py
```
