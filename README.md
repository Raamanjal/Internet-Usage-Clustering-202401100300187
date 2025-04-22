# Internet Usage Clustering

This project applies **unsupervised machine learning** (K-Means Clustering) to group users based on their internet usage behavior. The dataset includes information such as daily internet usage hours, types of site categories visited, and number of sessions per day. The goal is to automatically classify users into meaningful categories such as casual, moderate, and heavy internet users.

---

## Project Objectives

- Analyze internet usage data using machine learning techniques.
- Preprocess and scale features for better clustering results.
- Determine the optimal number of clusters using the Elbow Method.
- Apply **K-Means Clustering** to group users with similar online behavior.
- Visualize the clusters using data visualization tools.
- Analyze the behavioral patterns of each user cluster.

---

## Dataset Description

The dataset `internet_usage.csv` contains the following features:

| Feature Name             | Description                                                  |
|--------------------------|--------------------------------------------------------------|
| `daily_usage_hours`      | Average number of hours a user spends online per day         |
| `site_categories_visited`| Number of distinct website categories accessed by the user   |
| `sessions_per_day`       | Number of internet browsing sessions per day                 |

---

## Tools and Libraries Used

- **Python** 🐍
- `pandas` – For data loading and manipulation  
- `matplotlib` & `seaborn` – For data visualization  
- `sklearn` – For preprocessing and clustering (StandardScaler, KMeans)

---

## Methodology

1. **Data Preprocessing**
   - Load and clean data using `pandas`.
   - Standardize the features using `StandardScaler` to bring all values to a common scale.

2. **Determine Optimal Clusters**
   - Use the **Elbow Method** to find the best number of clusters (`k`).
   - Plot inertia vs. number of clusters to identify the "elbow point".

3. **Apply K-Means Clustering**
   - Fit the KMeans algorithm using the optimal `k`.
   - Assign each user to a cluster.

4. **Visualize and Analyze Clusters**
   - Use `seaborn.pairplot()` to visualize the cluster distribution.
   - Use `groupby()` to summarize each cluster's average behavior.

---

## Results

- Users were successfully clustered into distinct groups based on usage patterns.
- Each cluster reveals a different type of user:
  - Cluster 0: Light users
  - Cluster 1: Moderate users
  - Cluster 2: Heavy users

---
