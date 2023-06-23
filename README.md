# dataMiningLabTutorial
SENG 474 - Summer 2023

# Lab Task: Unsupervised Learning - K-means Clustering and the Elbow Method using RFM Analysis

## Objective
To perform RFM (Recency, Frequency, Monetary Value) analysis and apply the K-means clustering algorithm to identify distinct customer segments. Determine the optimal number of clusters using the Elbow Method.

## Materials Needed
1. Python programming environment (like Jupyter Notebook, Google Colab, etc.)
2. The purchase history dataset from [Kaggle](https://www.kaggle.com/datasets/mkechinov/ecommerce-purchase-history-from-electronics-store).

## Instructions

### 1. Download and Load the Dataset
Download the dataset from the provided Kaggle link and load it into your Python environment using Pandas' `read_csv` function.

### 2. Data Exploration
Explore the dataset using `head()`, `info()`, and `describe()` functions to understand its structure and statistical summary. Identify the relevant features for the RFM analysis (You'll need features related to customers (user_id), order date (event_time), and monetary value (price)).

### 3. Preprocessing
Handle missing data if any. Techniques can include deletion, mean/median/mode imputation, etc. Convert the 'event_time' column to DateTime type if it's not already.

### 4. Feature Engineering for RFM
- **Recency**: Calculate the number of days between the customer's latest purchase and the end of the period under study.
- **Frequency**: Compute the number of purchases made by each customer.
- **Monetary**: Calculate the total money spent by each customer.

### 5. Implement K-means
Apply the K-means clustering algorithm on your RFM data using Scikit-Learn's KMeans. Start by arbitrarily choosing a number of clusters (e.g., k=5).

### 6. Elbow Method
Apply the Elbow Method to find the optimal number of clusters. Plot a graph of the number of clusters (k) against the within-cluster sum of squares (WCSS). The "elbow" point on this graph represents the optimal number of clusters.

### 7. Interpret the Clusters
Reapply the K-means algorithm with the optimal number of clusters. Interpret each cluster by understanding its centroid and the characteristic of data points within it. Visualization can help with this interpretation.

### 8. Conclusion
Summarize your findings. What insights can be drawn from these clusters regarding customer purchasing behavior?

Remember, the goal of this lab exercise is to understand the process and results at each step. Each cluster represents a group of customers with similar Recency, Frequency, and Monetary values. These insights can inform strategies for customer retention, marketing, and more.

Good luck and have fun exploring the data! Let me know if you have any questions or need further assistance - I am walking around!
