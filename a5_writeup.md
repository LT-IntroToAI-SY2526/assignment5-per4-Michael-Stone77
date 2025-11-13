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

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?
Some things I learned through this assignment was how stacks and queues work as well as the differences between Depth first search and Breadth first search.  There weren't many challanges while implimenting the board class method but one problem came up during the BFS were it wouldn't do the search properly so I had to tweak it a little to get it on the right track but that was the only big issue I encountered. I tweacked it by taking some of the code from the depth first search and changing it to get the breadth first search functioning.


2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?
I can apply what I learned in this assignment to future programs by using the BFS and DFS for search algorithms or the board function could be used for other games if tweaked a little, games like chess or checkers could be made using it.  A real-world scenario where DFS and or BFS could be useful would be in things like networking where multiple nodes need to be connected and searched through in a given order, making it perfect for BFS or DFS depending on the network.


3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?
The Stack class works by only allowing the user to add or remove elements that are at the top of the of the stack and anything below is pushed down when a new element is added.  A Queue works different where it adds elements at the back and removes them at the front, allowing the front and back of the queue to be changed.  They are important to DFS and BFS becuase it's how they do there searches with our case being the board and DFS follows a stack while BFS follows a queue.  THe difference between LIFO and FIFO is that with LIFO, it can only add or remove something at the top of the stack and no where else while FIFO allows for things to be added at the back of the queue but removed from the start of it. LIFO is better suited for a DFS as it allows for every possibility to be run at the start before removing it and trying a new one while FIFO is better for BFS becuase it allows for a quick search through the queue which is what BFS is meant to do.  Using a stack changes the way a search algorithm explores possible solutions compared to a Queue is that a stack allows for a more in depth search compared to a queue which is a much faster look over of the algorithm.