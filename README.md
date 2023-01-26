# Imbalanced benchmarking set

## Description

The repository contains the benchmarking set for evaluating balancing methods in imbalanced binary classification. The set was proposed in my Engineering Thesis "The impact of data balancing on model behaviour with Explainable Artificial Intelligence tools in imbalanced classification problems".

## Data sources

The set is made of three main sources: *OpenML-100* benchmarking suite, *OpenML-CC18* benchmarking suite and the collection of datasets available in *imblearn* library in Python. It only contains continuous columns (categorical were removed). Each of the datasets contains at least 1000 rows and has Imbalance Ratio of at least 1.5. Additionaly, columns containing the same information were deleted.

This benchmarking set is also availble through the *edgaro* (link) package, which is the main result of my Engineering Thesis. It can be loaded using the following code:

```python
from edgaro.data.dataset_array import load_benchmarking_set
df = load_benchmarking_set()
```
## Datasets

The details of the datasets in the benchmarking set are presented in the table below:

| Dataset name        | Imbalance Ratio | Number of rows  | Number of columns | Source                            |
|---------------------|-----------------|-----------------|-------------------|-----------------------------------|
| spambase            | 1.54            | 4601            | 55                | OpenML-100, OpenML-CC18           |
| MagicTelescope      | 1.84            | 19020           | 10                | OpenML-100                        |
| steel-plates-fault  | 1.88            | 1941            | 13                | OpenML-100, OpenML-CC18           |
| qsar-biodeg         | 1.96            | 1055            | 17                | OpenML-100, OpenML-CC18           |
| phoneme             | 2.41            | 5404            | 5                 | OpenML-100                        |
| jm1                 | 4.17            | 10880           | 17                | OpenML-100, OpenML-CC18           |
| SpeedDating         | 4.63            | 1048            | 18                | OpenML-100                        |
| kc1                 | 5.47            | 2109            | 17                | OpenML-100, OpenML-CC18           |
| churn               | 6.07            | 5000            | 8                 | OpenML-CC18                       |
| pc4                 | 7.19            | 1458            | 12                | OpenML-100, OpenML-CC18           |
| pc3                 | 8.77            | 1563            | 14                | OpenML-100, OpenML-CC18           |
| abalone             | 9.68            | 4177            | 7                 | imblearn                          |
| us\_crime           | 12.29           | 1994            | 100               | imblearn                          |
| yeast\_ml8          | 12.58           | 2417            | 103               | imblearn                          |
| pc1                 | 13.40           | 1109            | 17                | OpenML-100, OpenML-CC18           |
| ozone-level-8hr     | 14.84           | 2534            | 72                | imblearn, OpenML-100, OpenML-CC18 |
| wilt                | 17.54           | 4839            | 5                 | OpenML-100, OpenML-CC18           |
| wine\_quality       | 25.77           | 4898            | 11                | imblearn                          |
| yeast\_me2          | 28.10           | 1484            | 8                 | imblearn                          |
| mammography         | 42.01           | 11183           | 6                 | imblearn                          |
| abalone\_19         | 129.53          | 4177            | 7                 | imblearn                          |
