# Breadth First search Algorithm
The Breadth First Search (BFS) algorithm is used to search a graph data structure for a node that meets a set of criteria. It starts at the root of the graph and visits all nodes at the current depth level before moving on to the nodes at the next depth level.

# Pseudocode 

BFS (G, s)                   //Where G is the graph and s is the source node
      let Q be queue.
      Q.enqueue( s ) //Inserting s in queue until all its neighbour vertices are marked.

      mark s as visited.
      while ( Q is not empty)
           //Removing that vertex from queue,whose neighbour will be visited now
           v  =  Q.dequeue( )

          //processing all the neighbours of v  
          for all neighbours w of v in Graph G
               if w is not visited 
                        Q.enqueue( w )             //Stores w in Q to further visit its neighbour
                        mark w as visited.
Traversing process

# Complexity
The time complexity of BFS is O(V + E), where V is the number of nodes and E is the number of edges
