# Assignment 1

1. Read Sections 1.1, 1.2, 1.3
2. **Graph coloring language**: Let us represent any undirected graph with a string of tuples where each tuple has the format (_id_, _color_) or (_id1, id2_). The tuple (_id1_, _id2_) indicates that there is an edge between node _id1_ and node _id2_. The tuple (_id_, _color_) indicates the color of the node id.
**Example**: The string _“(1,2),(1,red),(3,2),(2,green),(3,yellow)”_ represents a graph with three nodes 1,2 and 3. There are two edges, one between node 1 and node 2, and one between node 3 and node 2. Node 1 is colored red, node 2 is colored green, and node 3 is colored yellow.
- Write the grammar in ANTLR and generate the parse tree. Validate the grammar using different strings. 
