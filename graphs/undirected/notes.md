# 1. Graph Traversal
# Problem: Given an undirected graph represented by an adjacency list, implement the following:

# Depth-First Search (DFS): Write a function to perform DFS and return the nodes in the order they were visited.
# Breadth-First Search (BFS): Write a function to perform BFS and return the nodes in the order they were visited.

# DFS starting from node 'A'
# Expected output: ['A', 'B', 'D', 'E', 'F', 'C']

# BFS starting from node 'A'
# Expected output: ['A', 'B', 'C', 'D', 'E', 'F']


graph = {
    'A': ['B', 'C'],
    'B': ['A', 'D', 'E'],
    'C': ['A', 'F'],
    'D': ['B'],
    'E': ['B', 'F'],
    'F': ['C', 'E']
}




# 2. Shortest Path
# Problem: Implement Dijkstra’s algorithm to find the shortest path from a source node to all other nodes in a weighted graph.

# Shortest path from 'A' to all other nodes
# Expected output: {'A': 0, 'B': 1, 'C': 3, 'D': 4}

graph = {
    'A': {'B': 1, 'C': 4},
    'B': {'C': 2, 'D': 5},
    'C': {'D': 1},
    'D': {}
}


# 3. Minimum Spanning Tree
# Problem: Implement Kruskal’s algorithm to find the Minimum Spanning Tree (MST) of a weighted graph.
# Minimum Spanning Tree edges
# Expected output: [('A', 'B', 1), ('B', 'C', 2), ('C', 'D', 1)]

edges = [
    ('A', 'B', 1),
    ('A', 'C', 4),
    ('B', 'C', 2),
    ('B', 'D', 5),
    ('C', 'D', 1)
]

# 4. Topological Sort
# Problem: Implement a topological sort algorithm for a Directed Acyclic Graph (DAG).
# Topological sort of the graph
# Expected output: ['A', 'B', 'C', 'D'] or ['A', 'C', 'B', 'D']


graph = {
    'A': ['B', 'C'],
    'B': ['D'],
    'C': ['D'],
    'D': []
}

# 5. Strongly Connected Components (SCC)
# Problem: Implement Tarjan’s or Kosaraju’s algorithm to find all strongly connected components (SCCs) in a directed graph.
# Strongly connected components
# Expected output: [['A', 'B', 'C'], ['D', 'E', 'F']]

graph = {
    'A': ['B'],
    'B': ['C'],
    'C': ['A', 'D'],
    'D': ['E'],
    'E': ['F'],
    'F': ['D']
}




# 6. Cycle Detection
# Problem: Implement a function to detect whether a given graph contains a cycle.
# Detect cycle
# Expected output: True for graph_with_cycle, False for graph_without_cycle

graph_with_cycle = {
    'A': ['B'],
    'B': ['C'],
    'C': ['A']
}

graph_without_cycle = {
    'A': ['B'],
    'B': ['C'],
    'C': []
}



# 7. Hamiltonian Path/Circuit
# Problem: Implement a function to determine whether there is a Hamiltonian Path or Circuit in a graph.
# Check if there is a Hamiltonian Path
# Expected output: True for the given example

# Check if there is a Hamiltonian Circuit
# Expected output: True for the given example

graph = {
    'A': ['B', 'C'],
    'B': ['A', 'C', 'D'],
    'C': ['A', 'B', 'D'],
    'D': ['B', 'C']
}
