# Best-First Search vs A\*

**Best-First Search (Greedy):**  
This approach explores nodes by choosing the one closest to the goal using only the heuristic function `h(n)` (e.g., Manhattan distance). It often finds a path quickly but not necessarily the shortest one, since it ignores the cost of reaching that node. In our matrix example, Best-First Search may take “shortcuts” toward the goal but can result in longer or suboptimal paths.

**A\* Search:**  
A\* combines both the cost so far `g(n)` and the heuristic `h(n)` when selecting nodes, using the evaluation function `f(n) = g(n) + h(n)`. This ensures the algorithm not only heads toward the goal but also accounts for the path already taken. As a result, A\* always finds the shortest path (if one exists) at the expense of higher computation and memory usage. In practice, Best-First Search is faster but less reliable, while A\* is slower but guarantees optimal results.
