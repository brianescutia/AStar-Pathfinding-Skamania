# AStar-Pathfinding-Skamania
A* pathfinding algorithms for off-trail hiking GPS optimization (Skamania II) using admissible heuristics and runtime improvements.


# A* Pathfinding for Skamania II GPS

Final Project for ECS 170: Foundations of Artificial Intelligence.  
This project implements and optimizes A* pathfinding algorithms for a rugged terrain-based GPS used in the Skamania II hiking device.

##  Project Overview

The goal was to find optimal and efficient hiking routes using:
- **Exponential cost function:** `e^(h1 - h0)`
- **Squared difference cost function:** `1 + (h1 - h0)^2`

We designed admissible heuristics and improved runtime using A* variants while maintaining accuracy within 10% of optimal cost.

##  Features

- Implemented two admissible heuristics for different cost functions
- Created two A* search algorithms: `AStarExp` and `AStarSqdf`
- Developed `AStarExpImproved`, a faster variant using [insert variant, e.g., Bidirectional A*]
- Compared performance with Dijkstra's Algorithm
- Evaluated on 20+ benchmark terrains including Mt. St. Helens

##  Results

- ✅ `AStarExp` explored 50% fewer points than Dijkstra
- ✅ `AStarSqdf` explored 10% fewer points than Dijkstra
- ✅ `AStarExpImproved` ran 10%+ faster while keeping cost increase under 10%

##  Files

- `Brian_EscutiaProgrammingAssignment1.ipynb` – Full implementation and tests
- `Programming Assignment 1 - W25.pdf` – Project specifications

## 🛠 Tech Stack

- Python 3
- NumPy
- Matplotlib (for visualization)
- Jupyter Notebook

##  Real-World Impact

This project simulates off-trail hiking pathfinding – a practical use case for embedded GPS in remote areas. Optimization techniques reduce runtime on limited hardware like handheld GPS units.

## 📄 License

This project is open source under the MIT License.
