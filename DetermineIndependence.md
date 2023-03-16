## Determining Independence

In both Bayesian networks and Markov random fields (also known as Markov networks), independence between variables can be inferred by examining the graph structure. In the context of these graphical models, the concept of d-separation is used to determine conditional independence between variables.

**Bayesian Networks:** 

- In Bayesian networks, which are directed acyclic graphs (DAGs), d-separation is used to determine whether two sets of nodes (variables) are conditionally independent given a third set of nodes (observed variables).

- In a Bayesian network, two nodes X and Y are conditionally independent given a set of observed nodes Z if all paths between X and Y are blocked. A path is considered blocked if:

- The path contains a chain (X → Z → Y) or a fork (X ← Z → Y), and the middle node Z is observed.

- The path contains a collider (X → Z ← Y), and neither the middle node Z nor any of its descendants are observed.

- If all paths between X and Y are blocked given the observed nodes, then X and Y are conditionally independent given the observed nodes.

**Markov Random Fields:** 

- In Markov networks, which are undirected graphs, the concept of separation is used to determine conditional independence. In this case, we talk about separation instead of d-separation, as the graphs are undirected.

- In a Markov network, two nodes X and Y are conditionally independent given a set of observed nodes Z if all paths between X and Y are blocked by Z. A path is considered blocked if it contains a node from the set Z. In other words, X and Y are conditionally independent given Z if there is no path connecting them without passing through a node in Z.

To summarize, determining independence in Bayesian networks and Markov random fields involves examining the graph structure and applying the concepts of d-separation (for Bayesian networks) and separation (for Markov networks). By analyzing the paths between nodes and the observed nodes, you can infer conditional independence between variables in both types of graphical models.