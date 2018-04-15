# Introduction to Artificial Intelligence
### (Assignment 1  -  PacMan Search Trees)

#### 1. Overview
In this assignment, I edited the [search.py]() and [searchAgents.py]() files.

### 2. Implementation
On search.py I implemented:
1. depthFirstSearch(): can be tested with
  * `python pacman.py -l tinyMaze -p SearchAgent`
  * `python pacman.py -l mediumMaze -p SearchAgent`
  * `python pacman.py -l bigMaze -z .5 -p SearchAgent`
2. breadthFirstSearch(): can be tested with
  * `python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs`
  * `python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5`
  and it also should work for the 8-puzzle problem
  * `python eightpuzzle.py`
3. uniformCostSearch(): can be tested with
  * `python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs`
  * `python pacman.py -l mediumDottedMaze -p StayEastSearchAgent`
  * `python pacman.py -l mediumScaryMaze -p StayWestSearchAgent`
4. aStarSearch(): can be tested with
  * `python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic`

And on searchAgents.py I implemented:
1. The search problem CornersProblem: can be tested with
  * `python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem`
  * `python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem`
2. The cornersHeuristic for the CornersProblem: can be tested with
  * `python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.`
  this heuristic was proved to be consistent.
3. The foodHeuristic for the FoodSearchProblem: can be tested with
  * `python pacman.py -l trickySearch -p AStarFoodSearchAgent`