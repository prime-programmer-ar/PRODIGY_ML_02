# Prodigy InfoTech ML Internship - Task 02
# By: Zain Qamar

## Customer Segmentation using K-means Clustering

### Project Overview

This project uses the K-means clustering algorithm to group mall customers into distinct segments based on their annual income and spending score. The goal is to identify patterns and create targeted marketing strategies. This repository contains the solution for **Task 02** of the Prodigy InfoTec Machine Learning Internship.

---

### Workflow

1.  **Data Loading & Feature Selection:** The script loads the `Mall_Customers.csv` dataset and selects the `Annual Income (k$)` and `Spending Score (1-100)` columns for clustering.

2.  **Finding Optimal Clusters (Elbow Method):** To determine the best number of clusters, the Elbow Method is used. The script calculates the Within-Cluster Sum of Squares (WCSS) for a range of cluster numbers (1 to 10) and plots the results. The "elbow" in the plot indicates the optimal `k`.

3.  **K-means Clustering:** Based on the elbow plot, an optimal `k=5` is chosen. The K-means algorithm is then applied to group the customers into five distinct clusters.

4.  **Visualization:** A scatter plot is generated to visualize the five customer segments and their corresponding centroids, providing a clear view of the segmentation.

5.  **Output:** The script adds a `Cluster` column to the original dataset, assigning each customer to their respective segment, and saves the result as `Mall_Customers_Clusters.csv`.

---

### Visualizations

#### The Elbow Method
The plot below helps identify `k=5` as the optimal number of clusters.



#### Customer Clusters
This plot shows the final five customer segments based on their income and spending score.



*(Note: These images will be generated automatically when you run the script.)*

---

### How to Run

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/prime-programmer-ar/PRODIGY_ML_02
    cd PRODIGY_ML_02
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Prepare the dataset:**
    *   Create a folder named `dataset`.
    *   Place the `Mall_Customers.csv` file inside the `dataset` folder.

4.  **Execute the script:**
    ```bash
    python your_script_name.py
    ```
    The script will generate `elbow_plot.png`, `customer_clusters.png`, and `Mall_Customers_Clusters.csv`.

---

### Libraries Used
- Pandas
- Scikit-learn
- Matplotlib

### Dataset Used
- https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python


