# Customer Segmentation using Clustering

## Overview

This project focuses on customer segmentation based on their purchasing behavior. Using clustering techniques, we segment customers into distinct groups based on features like **Annual Income** and **Spending Score**. The goal is to identify customer segments that can be used for targeted marketing strategies, personalized product offerings, and improved customer retention.

## Dataset

The dataset used in this project is the **Mall Customers dataset** containing the following columns:

- **CustomerID**: Unique identifier for each customer
- **Genre**: Gender of the customer (Male/Female)
- **Age**: Age of the customer
- **Annual Income (k$)**: The annual income of the customer in thousands of dollars
- **Spending Score (1-100)**: A score assigned by the mall based on customer spending behavior

## Clustering Approach

1. **Preprocessing**:
   - The data is preprocessed by standardizing numerical features and one-hot encoding the categorical features (e.g., gender).
   
2. **Clustering Model**:
   - **Gaussian Mixture Model (GMM)** was applied to cluster the customers into **5 clusters**. The GMM is a probabilistic model that assumes the data is generated from a mixture of several Gaussian distributions.
   
3. **Evaluation**:
   - Several evaluation metrics such as **Silhouette Score**, **Calinski-Harabasz Index**, and **Davies-Bouldin Index** were used to evaluate the quality of the clusters.

4. **Cluster Profiles**:
   - Each cluster was analyzed based on its characteristics (e.g., income and spending score) to understand customer segments better.

## Key Insights

- **Cluster 1**: High Income, High Spending — Likely VIP customers.
- **Cluster 2**: Low Income, High Spending — Budget-conscious but willing to spend.
- **Cluster 3**: Medium Income, Low Spending — Cautious spenders.
- **Cluster 4**: Medium Income, Moderate Spending — Balanced consumers.
- **Cluster 5**: Low Income, Low Spending — Price-sensitive customers.

## Visualizations

The project includes various visualizations that help interpret the clustering results:

- **Pairwise scatter plots** to visualize relationships between customer features.
- **Box plots** to analyze feature distributions across clusters.
- **2D scatter plots** with clusters to visually assess separation and identify cluster patterns.

## Future Steps

- **Advanced Clustering**: Experimented with other clustering techniques such as **KMeans** or **DBSCAN** to compare results.
- **Targeted Marketing**: Develop targeted strategies for each cluster, such as offering premium products for high-spending customers.
- **Predictive Models**: Build predictive models for customer behavior, such as predicting spending based on income.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- sklearn

## Installation

To run the project, clone the repository and install the required libraries using `pip`:

```bash
git clone <repo-url>
cd <project-directory>
pip install -r requirements.txt
