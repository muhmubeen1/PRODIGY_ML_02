                            
# Customer Segmentation using K-Means Clustering

This project applies **K-Means clustering** to segment customers of a retail store based on their purchase history. The primary objective is to group customers into clusters based on shared behaviors, enabling better understanding and targeted marketing strategies.

## Project Overview

In this project, we:
- Preprocess customer data from the retail dataset.
- Scale the features for better performance in clustering.
- Apply the K-Means algorithm to cluster customers into different groups.
- Visualize and evaluate the clustering results.

You can view the repository for this project on GitHub: [PRODIGY_ML_02](https://github.com/muhmubeen1/PRODIGY_ML_02)

## Dataset

The dataset used for this project is `Mall_Customers.csv`, which contains the following columns:
- **CustomerID**: Unique ID for each customer.
- **Gender**: The gender of the customer.
- **Age**: The age of the customer.
- **Annual Income (k$)**: Annual income of the customer in thousand dollars.
- **Spending Score (1-100)**: A score assigned by the mall based on customer behavior and spending nature.

For the purpose of clustering, we renamed the "Spending Score" column to **Purchase** and selected the most relevant features from the dataset for clustering.

## Key Steps

### 1. Preprocessing
- **Label Encoding**: We used `LabelEncoder` to encode categorical columns like "Gender."
- **Scaling**: Since K-Means is sensitive to the scale of the features, we used `StandardScaler` to scale all features to have a mean of 0 and a standard deviation of 1.

### 2. K-Means Clustering
- The `KMeans` algorithm from `sklearn.cluster` was used to group customers into **5 clusters** based on their purchase behavior.
- We used the **Elbow Method** to determine the optimal number of clusters and the **Silhouette Score** to evaluate the quality of clustering.

### 3. Visualization
- A scatter plot was generated to visualize customer clusters, using color to differentiate between the clusters.

                    
                      
  

## How to Run

To run this project locally:
1. Clone the repository:
   ```bash
   git clone https://github.com/muhmubeen1/PRODIGY_ML_02.git
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook or the Python script.

## Future Improvements

- Perform feature engineering to derive additional features from the dataset.
- Explore other clustering techniques like **Hierarchical Clustering** or **DBSCAN** to compare results.
- Implement customer segmentation based on real-world business data from different domains.
                         
  
  
