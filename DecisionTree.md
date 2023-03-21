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

              Outlook
             / |   \
        Sunny Rainy Overcast
         /     |     \
    Humidity Windy  Play=2
     /   \             \
   High Normal       Play=1
    /      \
  Temp     Play=1
  /  \ 
 Hot Mild
  |   |
  |   | 
  |  Play=1
  |
  |
  |  
  |
 Cool 
  |
  |
  |
Play=1



