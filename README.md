# Imbalanced benchmarking set

## Description

The repository contains the benchmarking set for evaluating balancing methods in imbalanced binary classification. The set was proposed in my Engineering Thesis "The impact of data balancing on model behaviour with Explainable Artificial Intelligence tools in imbalanced classification problems".

## Data sources

The set is made of three main sources: *OpenML-100* benchmarking suite, *OpenML-CC18* benchmarking suite and the collection of datasets available in *imblearn* library in Python. It only contains continuous columns (categorical were removed). Each of the datasets contains at least 1000 rows and has Imbalance Ratio of at least 1.5.

Additionaly, columns containing the same information were deleted and, because of the size, the *protein_homo* dataset was randomly (preserving the class distribution) reduced to 30000 rows. 

This benchmarking set is also availble through the *edgaro* (link) package, which is the main result of my Engineering Thesis. It can be loaded using the following code:

```python
from edgaro.data.dataset_array import load_benchmarking_set
df = load_benchmarking_set()
```
## Datasets

The details of the datasets in the benchmarking set are presented in the table below:

| Dataset name       | Imbalance Ratio   | Number of rows  | Number of columns  |
|--------------------|--------|-------|-----|
| spambase           | 1.54   | 4601  | 55  |
| MagicTelescope     | 1.84   | 19020 | 10  |
| steel-plates-fault | 1.88   | 1941  | 13  |
| qsar-biodeg        | 1.96   | 1055  | 17  |
| phoneme            | 2.41   | 5404  | 5   |
| jm1                | 4.17   | 10880 | 17  |
| SpeedDating        | 4.63   | 1048  | 18  |
| kc1                | 5.47   | 2109  | 17  |
| churn              | 6.07   | 5000  | 8   |
| pc4                | 7.19   | 1458  | 12  |
| pc3                | 8.77   | 1563  | 14  |
| abalone            | 9.68   | 4177  | 7   |
| us\_crime          | 12.29  | 1994  | 100 |
| yeast\_ml8         | 12.58  | 2417  | 103 |
| pc1                | 13.40  | 1109  | 17  |
| ozone-level-8hr    | 14.84  | 2534  | 72  |
| wilt               | 17.54  | 4839  | 5   |
| wine\_quality      | 25.77  | 4898  | 11  |
| yeast\_me2         | 28.10  | 1484  | 8   |
| mammography        | 42.01  | 11183 | 6   |
| protein\_homo      | 111.36 | 30000 | 66  |
| abalone\_19        | 129.53 | 4177  | 7   |
