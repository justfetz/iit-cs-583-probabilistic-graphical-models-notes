## factor graphs

Consider a Markov network with three binary variables, X1, X2, and X3, where X1 and X2 are neighbors and X2 and X3 are neighbors. The factor graph for this network is shown below:
X1 -- f1 -- X2 -- f2 -- X3

In this factor graph, the variables are represented by circles and the factors are represented by squares. The edges between variables and factors indicate which variables are involved in which factors.

The factor graph for this Markov network shows that the joint probability distribution over the variables can be factorized as:

P(X1, X2, X3) = f1(X1, X2) * f2(X2, X3)

where f1 and f2 are the factors that involve the variables.

As for the parameterization of pairwise Markov random fields, pairwise Markov random fields are a type of Markov network that only allow interactions between pairs of variables. In a pairwise Markov random field, the energy function E(x) is parameterized in terms of a set of potential functions that represent the interactions between pairs of variables.

The pairwise Markov random field can be represented by a symmetric adjacency matrix W, where W_ij represents the strength of the interaction between variables i and j. The energy function E(x) for a pairwise Markov random field is defined as:

E(x) = -∑ W_ij * f_ij(x_i, x_j)

where f_ij(x_i, x_j) is the potential function that captures the interaction between variables i and j. The potential functions can take on a wide range of forms, depending on the specific application and the desired modeling assumptions.

In terms of parameter estimation, the potential functions and the strengths of the interactions can be learned from data using maximum likelihood estimation or other techniques. The learned parameters can then be used to perform inference and make predictions in the model.