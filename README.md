# DijkstraAndBellman_Comparison
The aim of this work is to do a comparative analysis of shortest path algorithms, to enable us know which is best for finding the shortest path from the source node to the destination node. And the objective are as follows: 

a. To implement Dijkstra and Bellman-ford shortest path algorithms. 

b. To determine the shortest path from the source node to the destination node. 

c. To evaluate the performance of the algorithms in terms of memory utilization and time complexity of the algorithms.


# Notes:
# Dijkstra 
1) The code calculates shortest distance, but doesn’t calculate the path information. We can create a parent array, update the parent array when distance is updated (like prim’s implementation) and use it show the shortest path from source to different vertices.

2) The code is for undirected graph, same dijkstra function can be used for directed graphs also.

3) The code finds shortest distances from source to all vertices. If we are interested only in shortest distance from the source to a single target, we can break the for the loop when the picked minimum distance vertex is equal to target (Step 3.a of the algorithm).

4) Time Complexity of the implementation is O(V^2). If the input graph is represented using adjacency list, it can be reduced to O(E log V) with the help of binary heap. Please see
Dijkstra’s Algorithm for Adjacency List Representation for more details.

5) Dijkstra’s algorithm doesn’t work for graphs with negative weight edges. For graphs with negative weight edges, Bellman–Ford algorithm can be used.

Output for Dijkstra’s algorithm:
Vertex   Distance from Source
0                0
1                4
2                12
3                19
4                21
5                11
6                9
7                8
8                14
