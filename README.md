Illinois Institute of Technology CS-535 Advanced Algorithms Notes

## CS - 583 Probabilistic Graphical Models Notes
```math
p(X=1|D) = \frac{\Gamma(2+3)}{\Gamma(2)\Gamma(3)} \left(\frac{1}{3}\right)^2 \left(\frac{2}{3}\right)^1 = 0.5319148936170212
```

`$p(X=1|D) = \frac{\Gamma(2+3)}{\Gamma(2)\Gamma(3)} \left(\frac{1}{3}\right)^2 \left(\frac{2}{3}\right)^1 = 0.5319148936170212$`

This repository contains my notes for a class on Probabilistic Graphical Models. The notes cover the following topics:

- Formulas
- I Maps
- P MAP (Perfect Map)
- Variable Ordering
- Probability Distributions
- Bayesian to Markov
- Markov to Bayesian
- d-separation and the conditioning set
- Laws of Probability

The notes include examples and explanations of each topic. 

### Formulas

The notes cover a variety of formulas related to Probabilistic Graphical Models, including:

- Bayes' Theorem
- Conditional Probability
- Joint Probability
- Posterior Distribution

### I Maps

The notes include examples and explanations of I Maps for both Bayesian Networks and Markov Networks. 

#### Bayesian Network I Map

```mermaid
graph TD
A
B
C
AC["AC (filled)"]
B-->AC
C-->AC
A-->B
```
#### Markov Network I Map
```mermaid
graph TD
A
B
C
AB["AB (filled)"]
BC["BC (filled)"]
A-->AB
B-->AB
B-->BC
C-->BC
```
## iit-pgm repository

