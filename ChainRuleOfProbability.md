## Chain Rule of Probability

-  The chain rule of probability is a basic rule of probability theory that allows us to calculate the joint probability of a set of random variables by breaking it down into a product of conditional probabilities.

-  Suppose we have a set of random variables X1, X2, ..., Xn. The chain rule of probability states that the joint probability of these variables can be written as a product of conditional probabilities, as follows:

-  ```P(X1, X2, ..., Xn) = P(X1) * P(X2 | X1) * P(X3 | X1, X2) * ... * P(Xn | X1, X2, ..., Xn-1)```

-  This rule tells us that the joint probability of a set of random variables can be decomposed into a product of conditional probabilities, each conditioned on the values of the previous variables in the sequence.

-  For example, suppose we have a coin that can land either heads (H) or tails (T), and we toss the coin twice. We can represent the outcome of each toss by random variables X1 and X2, respectively. The joint probability distribution of X1 and X2 can be calculated using the chain rule of probability as follows:

- ``` P(X1, X2) = P(X1) * P(X2 | X1)```

where:

P(X1) is the probability of the first toss, which is 0.5 for both H and T.
P(X2 | X1) is the probability of the second toss, given the outcome of the first toss. This is also 0.5 for both H and T, but depends on the outcome of X1.
Using this rule, we can calculate the joint probability distribution of X1 and X2 as:

P(H, H) = P(H) * P(H | H) = 0.5 * 0.5 = 0.25
P(H, T) = P(H) * P(T | H) = 0.5 * 0.5 = 0.25
P(T, H) = P(T) * P(H | T) = 0.5 * 0.5 = 0.25
P(T, T) = P(T) * P(T | T) = 0.5 * 0.5 = 0.25

This gives us the complete joint probability distribution of the two coin tosses.
