# WTF is an I Map

## Bayesian

// Bayesian Network Minimal I Map example
\require{enclose}
\enclose{circle}[mathcolor="blue"]{A} \rightarrow \enclose{square}[mathcolor="green",mathbackground="#FFFFCC"]{AC}
C \rightarrow AC
\enclose{circle}[mathcolor="blue"]{B} \rightarrow \enclose{square}[mathcolor="green",mathbackground="#FFFFCC"]{AC}
A \rightarrow B


* A Bayesian Network is a probabilistic graphical model that represents a set of variables and their conditional dependencies using a directed acyclic graph (DAG).
The Minimal I Map for a Bayesian Network is a graph that preserves the essential dependence relations among the variables, while minimizing the number of edges.
In the example, the nodes A, B, and C represent the variables in the Bayesian Network, and the node AC represents the essential dependence relation between A and C.

* In the context of graphical models, a minimal I-Map (Independence Map) is a graph that represents the set of all conditional independence statements implied by a given Bayesian or Markov structure.

* For a Bayesian network structure, a minimal I-Map is a directed acyclic graph (DAG) that represents the conditional independence relationships among the variables in the network. In a Bayesian network, the variables are represented as nodes in the graph, and the edges between the nodes represent direct dependencies between the variables. The minimal I-Map for a Bayesian network structure is the smallest DAG that contains all the conditional independence statements implied by the structure.

// Markov Network Minimal I Map example
graph MarkovNetwork {
  node [shape=circle]
  A;
  B;
  C;
  node [shape=square,style=filled]
  AC;
  B -- AC;
  C -- AC;
  A -- B;
}


* For a Markov network structure, a minimal I-Map is an undirected graph that represents the conditional independence relationships among the variables in the network. In a Markov network, the variables are represented as nodes in the graph, and the edges between the nodes represent direct dependencies between the variables. The minimal I-Map for a Markov network structure is the smallest undirected graph that contains all the conditional independence statements implied by the structure.

* The concept of minimal I-Map is important in graphical modeling because it allows us to represent the complex dependencies among variables in a compact and intuitive way. It also provides a way to identify the set of conditional independence relationships that are necessary and sufficient for inference and learning in the model.
