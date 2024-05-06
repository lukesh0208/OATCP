1. Import necessary libraries: <iostream>, <limits.h>, <queue>, <string.h>.
2. Define the macro V representing the number of vertices in the graph.
3. Define a function bfs that performs Breadth-First Search (BFS) to find a path from source s to sink t in the residual graph.
   -Initialize an array visited to keep track of visited vertices.
   -Create a queue q and enqueue the source vertex s.
   -Mark s as visited and set its parent as -1.
   -While the queue is not empty:
    -Dequeue a vertex u.
    -Iterate through all vertices v.
      -If v is not visited and there is a residual capacity from u to v:
        -If v is the sink t, set its parent as u and return true.
        -Enqueue v, mark it as visited, set its parent as u.
 -If no path is found, return false.
4. Define a function fordFulkerson that implements the Ford-Fulkerson algorithm to find the maximum flow from source s to sink t in the given graph.
   -Create a residual graph rGraph as a copy of the original graph.
   -Initialize an array parent to store the parent of each vertex in the augmenting path.
   -Initialize max_flow as 0.
   -While there exists a path from source s to sink t in the residual graph:
     -Find the minimum residual capacity along the augmenting path.
     -Update the residual capacities along the augmenting path.
     -Update the maximum flow by adding the path flow.
   -Return max_flow.
5. In the main function:
   -Define the capacity graph as a 2D array graph.
   -Call the fordFulkerson function with the graph, source 0, and sink 5.
   -Print the maximum flow obtained.