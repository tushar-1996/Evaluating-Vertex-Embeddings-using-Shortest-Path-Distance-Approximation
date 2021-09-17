## Results

| Embedding Type        | Our results inittrain| Our results gentrain1| Paper repo results  | Paper official results |
| -------------         |:-------------:       |  -----               | -----:              | ---                    |
|                       |  MAE       RMSE      |  MAE       RMSE      |  MAE       RMSE     |  MAE       RMSE        |
| Average               | 0.064      0.253     | 0.037      0.193     | 0.088      0.298    | 0.118                  |
| Concatenation         | 0.172      0.415     | 0.166      0.408     | 0.163      0.406    | 0.258                  |
| Hadamard              | 0.158      0.398     | 0.124      0.355     | 0.144      0.381    | 0.217                  |
| Substraction          | 0.291      0.554     | 0.270                | 0.250      0.515    | 0.197                  |

## Summary Inittrain
| Number of nodes       | Number of Edges       | Number of training pairs| Number of testing pairs |
| -------------         |:-------------:        | -----:                  | ---                     |
| 4039                  | 88234                 | 1022640                 | 109978                  |

## Summary Gentrain01
| Number of nodes       | Number of Edges       | Number of training pairs| Number of testing pairs |
| -------------         |:-------------:        | -----:                  | ---                     |
| 4039                  | 88234                 | 1031093                 | 113427                  |

- The used training and testing data in inittrain come from the original paper repository
- The results were measured with the testing set after 15 epochs of training
- Learning rate was default SGD learning rate from keras (0.01)