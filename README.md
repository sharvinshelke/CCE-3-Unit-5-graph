CCE-3-Unit-5-graph
Industrial Sensor Network Using Kruskal's Algorithm

1. Problem Statement
Represent industrial sensors as vertices and possible wiring connections as edges with installation costs. Apply Kruskal's algorithm to connect all sensors at minimum total installation cost.

2. Aim
To implement Kruskal's algorithm in C++ to find the Minimum Spanning Tree (MST) of an industrial sensor network.

3. Objectives

Represent industrial sensors and wiring connections using a graph.
Arrange wiring connections in increasing order of installation cost.
Select minimum-cost connections without forming cycles.
Calculate the minimum total installation cost.

4. Theory
Kruskal's algorithm is a greedy algorithm used to find a Minimum Spanning Tree (MST) in a connected, weighted, undirected graph.
It sorts all edges by cost and selects the lowest-cost edge that does not form a cycle. The process continues until all vertices are connected using "V - 1" edges, where "V" is the number of vertices.
A Disjoint Set Union (DSU) data structure is used to detect cycles efficiently.

5. Algorithm

1. Start the program.
2. Read the number of sensors and possible wiring connections.
3. Store each connection with its source, destination and installation cost.
4. Sort all connections in ascending order of cost.
5. Select the lowest-cost connection that does not form a cycle.
6. Repeat until "V - 1" connections are selected or no more valid connections remain.
7. If all sensors are connected, display the selected connections and minimum total cost.
8. Otherwise, display a message that all sensors cannot be connected.
9. Stop.

6. Input Format

First, enter the number of sensors.
Next, enter the number of possible wiring connections.
For each connection, enter the source sensor, destination sensor and installation cost.
Sensor numbers start from 1.
Installation costs must be non-negative.

7. Sample Input

4  
5
1 2 10
1 3 6
1 4 5
2 4 15
3 4 4

8. Sample Output

Minimum-cost wiring connections:
Sensor 3 - Sensor 4 : Cost = 4
Sensor 1 - Sensor 4 : Cost = 5
Sensor 1 - Sensor 2 : Cost = 10

Minimum Total Installation Cost = 19

9. Applications

 Industrial sensor network installation.
 Factory automation wiring.
 Connecting monitoring and control units.
 Designing cost-effective communication networks.
 Planning minimum-cost infrastructure connections.

10. Advantages

 Minimizes total wiring installation cost.
 Avoids unnecessary connections and cycles.
 Works with weighted graphs.
 Can identify when the given network cannot connect all sensors.

11. Conclusion

The Industrial Sensor Network program uses Kruskal's algorithm to determine the minimum-cost wiring connections required to connect all industrial sensors. It selects the lowest-cost edges without forming cycles and calculates the minimum total installation cost.

