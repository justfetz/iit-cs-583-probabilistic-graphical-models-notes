## Decision Trees

### Table

| Outlook   | Temp  | Humidity | Windy  | Play |
|-----------|-------|----------|--------|------|
| Sunny     | Hot   | High     | FALSE  | 2    |
| Sunny     | Hot   | High     | TRUE   | 3    |
| Overcast  | Hot   | High     | FALSE  | 1    |
| Rainy     | Mild  | High     | FALSE  | 1    |
| Rainy     | Cool  | Normal   | FALSE  | 1    |
| Rainy     | Cool  | Normal   | TRUE   | 1    |
| Overcast  | Cool  | Normal   | TRUE   | 1    |
| Sunny     | Mild  | High     | FALSE  | 1    |
| Sunny     | Cool  | Normal   | FALSE  | 1    |
| Rainy     | Mild  | Normal   | FALSE  | 1    |
| Sunny     | Mild  | Normal   | TRUE   | 1    |
| Overcast  | Mild  | High     | TRUE   | 1    |
| Overcast  | Hot   | Normal   | FALSE  | 1    |
| Rainy     | Mild  | High     | TRUE   | 1    |


### The Tree with Observations

                             Outlook (14)
                            /  |   \
                           /   |    \
                      Sunny  5     Overcast (4)
                        / \          /  \
                       /   \        /    \
              Humidity 2   Windy 3  Yes (4)
                /   \                /   \
               /     \              /     \
            High   Normal          /      \
                                Humidity 2  Windy
                                  /  \     /   \
                                 /    \   /     \
                                High Normal No (1)
                                             /   \
                                            /     \
                                           /       \
                                        Windy      Yes (3)
                                          /   \
                                         /     \
                                        /       \
                                       FALSE    TRUE (2)


