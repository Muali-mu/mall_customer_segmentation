# 🛍️ Customer Segmentation using Clustering

## 📌 Project Overview
This project performs **customer segmentation** using the popular **Mall Customer dataset**.  
We apply clustering algorithms to group customers based on their **Annual Income** and **Spending Score**.  
The goal is to identify distinct customer groups to help businesses target marketing strategies more effectively.  

---

## 🚀 Steps Followed

### 1. Data Loading
- Dataset is loaded directly from a GitHub raw CSV file.
- Columns considered:  
  - `Annual Income (k$)`  
  - `Spending Score (1-100)`

### 2. Feature Scaling
- Data is standardized using **StandardScaler** from `sklearn`.
- Scaling ensures that income and spending score contribute equally to clustering.

### 3. K-Means Clustering
- **Elbow Method** is used to determine the optimal number of clusters (k).  
- The elbow graph suggests **k = 5** clusters.  
- Customers are clustered accordingly.

### 4. Cluster Visualization
- Clusters are plotted in **2D scatter plots** using Seaborn.
- Each cluster is represented with a different color for clarity.

### 5. Cluster Analysis
- Average **Annual Income** and **Spending Score** are calculated for each cluster.
- This helps interpret characteristics of each customer segment.

### 6. DBSCAN (Bonus)
- Density-Based Spatial Clustering (**DBSCAN**) is applied.  
- Unlike K-Means, DBSCAN can find clusters of arbitrary shapes and also detect noise points (`-1` cluster).  
- Clusters are visualized and analyzed.

---

## 📊 Results

- **K-Means produced 5 meaningful clusters**:  
  - Low income, low spenders  
  - Low income, high spenders  
  - High income, low spenders  
  - High income, high spenders  
  - Average income and spending customers  

- **DBSCAN** detected clusters based on density, but some customers were classified as noise (`-1`).  

---

## 🛠️ Tools & Libraries Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 📈 Visualizations
- **Elbow Method plot** – helps select the best number of clusters.  
- **K-Means scatter plot** – shows customer segments clearly.  
- **DBSCAN scatter plot** – displays density-based clusters.  

---

## ✅ Conclusion
- **K-Means** worked well for this dataset, providing 5 clear clusters.  
- **DBSCAN** is useful when clusters are irregular in shape but may mark many points as noise.  
- Businesses can use these insights to:  
  - Target marketing campaigns  
  - Identify premium customers  
  - Improve customer retention strategies  
