# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

BFS becuase it checks each branch as it gets futher down the tree. DFS checks a singular pathway all the way which can be inefficient due to the large amount of potential solutions. On the otherhand, BFS checks the individual levels of each pathway before advancing further down the tree which is more efficient for sudoku and scenarios with becuase it checks multiple pathways at a time instead of long potential pathways individually as DFS does.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

The data structures impact the algorithms because each structure iterates through the data differently, which can cause the program to run longer or shorter depending on the objective of the program. There are different types or varieties of these data structures such as deques, heaps, and hashes.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

One implementation to adapt to a larger sudoku puzzle would be increasing the grid size or having a variable that holds the grid size therefore it could adapt to a larger puzzle without having to change the code. These can be applied to real-world problem-solving by using the FIFO or FILO structures to iterate through possibilities when solving a problem.