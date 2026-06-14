# Retail Customer Segmentation using K-Means Clustering

This repository contains my submission for **Task-02** of the Machine Learning Internship at **Prodigy InfoTech**.

## Project Overview
The objective of this task is to create an unsupervised K-Means Clustering algorithm to group customers of a retail store based on their purchase history metrics (Annual Income and Spending Score).

## Dataset
The model uses the [Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) from Kaggle. It contains basic demographic data for 200 mall customers:
* CustomerID
* Gender
* Age
* Annual Income (k$)
* Spending Score (1-100)

## Implementation Steps
1. **Data Exploration:** Loaded and inspected the customer profile distributions.
2. **Feature Selection:** Extracted `Annual Income` and `Spending Score` as the primary grouping variables.
3. **Elbow Method:** Ran a loop tracking WCSS across 1-10 clusters to identify the sharp "elbow" optimal point at **K=5**.
4. **Model Training:** Fitted the `KMeans` algorithm with 5 clusters using `k-means++` initialization.
5. **Visualization:** Plotted a comprehensive scatter plot mapping all 5 colorful customer segments along with their bright yellow cluster centroids.

## Identified Segments
* **Cluster 1:** Average Income, Average Spending
* **Cluster 2:** High Income, High Spending (Primary Target Group)
* **Cluster 3:** Low Income, High Spending
* **Cluster 4:** High Income, Low Spending
* **Cluster 5:** Low Income, Low Spending

## Tech Stack
* Python 3
* Jupyter Notebook
* Pandas & NumPy
* Scikit-Learn
* Matplotlib
