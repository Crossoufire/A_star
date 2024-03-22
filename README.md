# A* Algorithm Interactive Visualization
- This repository contains an interactive Python code using matplotlib for visualizing the A* algorithm
- A* is a very popular pathfinding algorithm used in various applications, including robotics, gaming, and navigation systems

## Overview
- The A* algorithm aims to find the shortest path between two points on a grid by considering both the cost to reach a node from the start point 
(the `g_cost`) and an estimate of the cost to reach the goal from that node (the `h_cost`)
- The algorithm then selects the most promising nodes to explore next based on a combination of these costs

## Features
- **Interactive Visualization:** This code provides an interactive visualization of the A* algorithm using Matplotlib
- **Add obstacles:** You can click on grid cells to add or remove obstacles and start the algorithm to see it in action
- **Customizable Grid:** You can specify the grid size as well as the start and end points to adapt the visualization to different scenarios
- **Manhattan Distance Heuristic:** The algorithm uses Manhattan distance to estimate the cost from each node to the goal

## Requirements
- Python 3.7+
  - Matplotlib
  - NumPy

## Installation
- Clone the repository
```bash
git clone https://github.com/Crossoufire/A-star.git
```
- Install the required dependencies
```bash
pip install -r requirements.txt
```

## Usage
- You can customize the `grid size`, the `start point`, and `end points` variables in the `__main__` block
- Run the script
```bash
python AStar.py
```
- Use `Left click` on grid cells to add an obstacle, and `right click` to remove it
- Press `spacebar` to start the algorithm

## Example
```python
if __name__ == "__main__":
    grid_nodes = GridNodes(15, 15)

    start_node: Node = Node(2, 2)
    end_node = Node(12, 12)

    A_Star(grid_nodes, start_node, end_node)

    plt.show()
```

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements
The A* algorithm implementation in this code is inspired by various online resources and textbooks on algorithms and pathfinding.
