# CryptoClustering

## Introduction
This repository explores the clustering of cryptocurrencies using K-means and Principal Component Analysis (PCA). Aiming to identify optimal cluster counts and understand the impact of dimensionality reduction on clustering.

## Files and Setup

### Data Preparation:
1. Use StandardScaler from scikit-learn to normalize the data.
2. Create a DataFrame with the scaled data, setting "coin_id" as the index.

### Elbow Method for Optimal k:
1. Create a list of k values from 1 to 11.
2. Compute inertia for each k using K-means.
3. Plot an elbow curve to find the optimal k.
4. Answer the question: What is the best value for k?

### K-means Clustering (Original Scaled Data):
1. Initialize K-means model with the best k.
2. Fit the model and predict clusters.
3. Add predicted clusters to a copy of the original data.
4. Create a scatter plot using hvPlot.

### PCA for Dimensionality Reduction:
1. Perform PCA on the original scaled data.
2. Retrieve explained variance for each principal component.
3. Answer the question: What is the total explained variance of the three principal components?
4. Create a DataFrame with PCA data, setting "coin_id" as the index.

### Elbow Method for Optimal k (PCA Data):
1. Create a list of k values from 1 to 11.
2. Compute inertia for each k using K-means on PCA data.
3. Plot an elbow curve to find the optimal k.
4. Answer the question: What is the best value for k when using the PCA data? Does it differ from the best k value found using the original data?

### K-means Clustering (PCA Data):
1. Initialize K-means model with the best k from PCA.
2. Fit the model and predict clusters on PCA data.
3. Add predicted clusters to a copy of the PCA data.
4. Create a scatter plot using hvPlot.

## Conclusion:
Answer the question: What is the impact of using fewer features to cluster the data using K-Means?
