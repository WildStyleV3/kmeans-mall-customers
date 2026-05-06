# K-Means Customer Segmentation

Customer segmentation on the Mall Customers dataset using K-Means clustering.
Coursework for Data Mining (Prof. Sebastián Moreno, UAI).

## Approach

- EDA and standardization of Age, Annual Income, and Spending Score.
- Outlier detection with Local Outlier Factor (LOF), grid search over `n_neighbors ∈ {5, 10, 20, 30, 50}`.
- Outliers retained after z-score check (none exceed ±3 SD).
- Optimal k=5 selected via elbow method combined with visual inspection and commercial interpretability.

## Results

Five customer segments identified:

1. Low income — low spending
2. Moderate income — high spending
3. Premium (high income — high spending)
4. High income — low spending (priority for targeted marketing)
5. Mid income — mid spending

## Stack

Python · pandas · scikit-learn · plotnine

## Run

```bash
pip install pandas scikit-learn plotnine seaborn
jupyter notebook kmeans_mall_customers.ipynb
```
