# High Performance Algorithms in C++
A curated list of Algorithms and their respectable Big O notation.

## Bellman-Forth Shortest Path
created by Richard Bellman and Lester Ford, Jr., determines the shortest path from a start vertex to each vertex in a graph. For each vertex, the Bellman-Ford algorithm determines the vertex's distance and predecessor pointer. A vertex's distance is the shortest path distance from the start vertex. A vertex's predecessor pointer points to the previous vertex along the shortest path from the start vertex. The runtime for this algorithm is O(V*E) because of the outer loop executes V-1 times. In each outer loop execution, the algorithm visits each vertex and follows the subset of edges to adjacent vertices, following a total of E edges across all loop executions.

## Dijkstra's Shortest Path 
created by Edsger Dijkstra, determines the shortest path from a start vertex to each vertex in a graph. For each vertex, Dijkstra's algorithm determines the vertex's distance and predecessor pointer. A vertex's distance is the shortest path distance from the start vertex. A vertex's predecessor pointer points to the previous vertex along the shortest path from the start vertex. In each outer loop execution, popping the vertex from the queue requires searching all vertices in the list, which has a runtime of O(V). For each vertex, the algorithm follows the subset of edges to adjacent vertices; following a total of E edges across all loop executions. Given E < V2, the runtime is O(V*V + E) = O(V2 + E) = O(V2). Implementing the queue using a fast heap data structure reduces the runtime to O(E + V log V). However, If the unvisited vertex queue is implemented using a list, the runtime for Dijkstra's shortest path algorithm is O(V2).

## 
