# Pathfinding Algorithms Visualizer

All algorithms are implemented as Graph Search, i.e., already visited spots will not be considered again.

## Uninformed (using no heuristics) search algorithms:
* Breadth-First-Serch
* Depth-First-Search
* Uniform-Cost-Search (Dijkstra)

## Informed (using heuristics) search algorithms:
* Greedy-Best-First-Search
* A*-Search

The heuristic used here is the L-shape distance, i.e., abs(x_cell - x_goal) + abs(y_cell - y_goal). It can be easily seen that this heuristic satisfies the following triangle inequality and is thus "consistent" which is the requirement for A*-Graph-Search to be optimal, i.e., to always find the shortest solution path (if a solution path exists):

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; heuristic(cell) <= costs(cell, cell') + heuristic(cell'),
			
where cell' is a neighbour of cell and costs(cell, cell') are the costs to get from cell to cell' (which is 
always 1).

<img src="demo-images/demo_bright_mode.PNG">

<img src="demo-images/demo_dark_mode.PNG"> 
