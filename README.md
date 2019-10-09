#AStarTilePuzzle

This repository uses the A* algorithm to solve tile puzzles of N size.

The puzzle is set using the Puzzle class with a parameter N specifying the size of the puzzle. The class prompts the user for the start of the puzzle in the form of: 

```
_ 2 1
3 4 5
6 7 8
```

The class then prompts the user for the goal state in the form of: 

```
_ 1 2
3 4 5
6 7 8
```

Along with this, the class also has: 
- Method f (The f value using the heuristic function and G which is depth)
- Method h (Simple heuristic function - Tile Difference)
- Method process (Execution of the A* algorithm with open and closed list)


As the puzzle is solved, nodes are generated for each state. The node is created using the Node class. The node class contains: 
- Method get_childern (Returns all possible moves at the current time-step)
- Method child (Generated the child)
- Method find (Finds x and y values for a specific value)

Using this, the N tile puzzle is solved. 
