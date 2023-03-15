## Convert Bayesian Network to Markov Network

A **Bayesian network (BN)** and a **Markov network (MN)**, also known as a Markov random field, are both graphical models used to represent the probabilistic relationships among a set of random variables. While BNs are directed acyclic graphs (DAGs) with nodes representing random variables and directed edges capturing conditional dependencies, MNs are undirected graphs where the nodes represent random variables and the edges represent undirected relationships between the variables.

To convert a Bayesian network into a Markov network, you can follow these steps:

**Moralization:** The first step involves turning the directed edges in the Bayesian network into undirected edges, which creates an undirected graph. To do this, you connect all pairs of nodes that have a common child, creating an undirected edge between them if it doesn't already exist. This process is called "moralization" because it creates an undirected relationship between the parents of a common child, as if they were "married."

**Removal of directed edges:** Once you have created the undirected edges between parents of common children, remove the direction from all remaining directed edges in the original BN. Now you have an undirected graph representing the relationships between the variables.

**Potential functions:** The next step is to represent the conditional probability distributions (CPDs) from the Bayesian network as potential functions in the Markov network. In a Markov network, each clique of nodes (a fully connected subgraph) is associated with a potential function that measures the compatibility of the assignments to the variables in the clique. For each CPD in the Bayesian network, create a potential function over the corresponding clique in the Markov network, which consists of the variable and its parents in the original BN.

For example, if the Bayesian network has a CPD $P(X|Y, Z)$, create a potential function $\psi(X, Y, Z)$ in the Markov network. The values of the potential function are determined by the CPD, e.g., $\psi(x, y, z) = P(x|y, z)$ for all possible values of X, Y, and Z.

**Normalize:** Note that unlike Bayesian networks, the potential functions in a Markov network don't directly represent probabilities. Instead, the joint probability distribution over all variables can be derived from the product of all potential functions, normalized by a partition function (Z). The partition function is the sum of the product of potential functions over all possible variable assignments.

$P(X_1, X_2, \dots, X_n) = \frac{1}{Z} \times \prod_i \psi_i(C_i)$,

where $\prod_i \psi_i(C_i)$ is the product of all potential functions, $C_i$ represents the cliques, and $Z$ is the partition function that ensures the probabilities sum to 1.

Now you have converted a Bayesian network into a Markov network, representing the same joint distribution, but using undirected relationships and potential functions instead of directed edges and conditional probability distributions.
