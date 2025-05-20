# X-Val-vs-Hold-Out-Testing
The objective of this assignment is to assess when it is beneficial to use cross-validation instead of hold-out testing and when it is not. The dataset to be used in this assignment is provided in the csv file diabetes_70k.csv. This dataset is derived from the UCI dataset here: https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators.
# Key Results:
#### Relative merits of X-val and Hold Out evaluations:
|                       X-val                 |                 Hold Out                 |
|---------------------------------------------|------------------------------------------|
|Rigorous and reliable as it averages out the accuracy over kfolds and reduces the impact of one-odd data-split| Suitable for large datasets were a large test set is good enough for estimating accuracy |
|More suitable for smaller sets vs HO, maximises the use of limited data| Suitable for deploying large models in real time where it will be computationally inefficient to run evaluations ktimes|
|Lower variance in accuracy estimates due to moderating effect of averaging|High variance in smaller datasets because of one split strategy, its simplicity and practicality are best for larger datasets and complex models such as deep learning|
