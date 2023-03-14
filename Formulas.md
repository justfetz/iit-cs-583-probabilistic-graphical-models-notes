# Formulas

### Bayes Theorm
$P(A | B) = \frac{P(B | A) \cdot P(A)}{P(B)}$

### Chain Rule of Probability
$P(A_1, A_2, ..., A_n) = P(A_1) \cdot P(A_2 | A_1) \cdot P(A_3 | A_1, A_2) \cdots P(A_n | A_1, A_2, ..., A_{n-1})$

### Law of Total Probability
$P(B) = \sum_i P(B | A_i) \cdot P(A_i)$

### Conditional Probability
$P(A | B) = \frac{P(A \cap B)}{P(B)}$

### Expected Value
$E(X) = \sum_i x_i \cdot P(X = x_i)$

### Variance
$Var(X) = E((X - \mu)^2) = \sum_i (x_i - \mu)^2 \cdot P(X = x_i)$

### Standard Deviation
$\sigma_X = \sqrt{Var(X)}$

### How to make a matrix
$$
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{pmatrix}
$$

### How to make a table
|   | Column 1 | Column 2 |
|---|----------|----------|
| Row 1 | 1 | 2 |
| Row 2 | 3 | 4 |


### Conditional Probability Distribution:
$$P(A|B)$$

### Marginal Probability Distribution:
$$P(A)$$

### Gaussian (Normal) Distribution:
$$P(x) = \frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}}$$

### Bernoulli Distribution:
$$P(x) = \begin{cases} 1-p &\text{if } x=0\ p &\text{if } x=1 \end{cases}$$

### Binomial Distribution:
$$P(x) = {n\choose x}p^x(1-p)^{n-x}$$

### Poisson Distribution:
$$P(x) = \frac{\lambda^x e^{-\lambda}}{x!}$$

### Exponential Distribution:
$$P(x) = \lambda e^{-\lambda x}$$