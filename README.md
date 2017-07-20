# GraphLabsSuite.Core.Graphs
The graph library of the GraphLabs project

### Installation
* npm install graphlabs.core.graphs

### Content
* JSON types
** GraphJSON - representation of the whole graph in JSON format
** VertexJSON - representation of the vertex in JSON format
** EdgeJSON - representation of the edge in JSON format

* Interfaces
** IGraph - interface for working with graph functions
** IVertex - interface for working with vertex functions
** IEdge - interface for working with edge functions
** IWeightedEdge - interface for working with weighted edges

* Main classes
** Vertex
*** isAdjacent - checks whether the second vertex is adjacent to the given one
*** isIncident - checks whether the edge is incident to the given vertex
** Edge
*** isIncident - checks whether the vertex is incident to the given edge
** UndirectedEdge
** DirectedEdge
** DirectedWeightedEdge
** Graph
*** addEdge - adds the edge to the graph
*** removeEdge - removes the edge from the graph
*** getEdge - gets the edge by the vertices incident to it
*** addVertex - adds the vertex to the graph
*** removeVertex - removes the vertex to the graph
*** getVertex - gets the vertices by the name requested
*** union - returns the result of union operation with another graph
*** unionN - static extension of union operation for N graphs
*** intersect - returns the result of intersect operation with another graph
*** intersectN - static extension of intersect operation for N graphs
*** complement - returns a complement graph to the given one
*** buildSCC - returns strongly connected components of the graph
*** print - prints the graph to the console
*** toString - returns the string view of the graph
*** clone - returns a deep clone of the graph
** UndirectedGraph
*** buildMDS - returns minimal dominating sets of the graph
** DirectedGraph
** DirectedWeightedGraph

* Auxiliary classes
** GraphToJSONConverter - converts graph to JSON format and controversially
** VertexToJSONConverter - converts vertex to JSON format and controversially
** EdgeToJSONConverter - converts edge to JSON format and controversially
** GraphSerializer
*** serialize - returns string representation of the graph
*** deserialize - returns graph from its string representation
** GraphGenerator
*** generate - generates an instance of Graph type with random vertex and edge numbers