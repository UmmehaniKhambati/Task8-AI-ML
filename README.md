#Task8-AI-ML
#K-Means Clustering

# Objective
Performed unsupervised clustering on the Mall Customers dataset using K-Means to identify customer segments.

# Dataset
- File: Mall_Customers.csv  
- Rows: 200 | Columns: 5  
- Features used: Age, Annual Income (k$), Spending Score (1–100)  

# Workflow
1. Loaded dataset → 200 rows, no missing values.  
2. Dropped CustomerID, selected numerical features.  
3. Scaled features using StandardScaler.  
4. Elbow Method → optimal K = 5.  
5. Applied K-Means, assigned cluster labels.  
6. Visualized clusters (Annual Income vs Spending Score, PCA 2D).  
7. Evaluated using Silhouette Score.

# Results
- Elbow Curve: Clear bend at K=5.  
- Silhouette Score: 0.41 → fair clustering structure.  
- Customer Segments:  
  - Cluster 0 → Medium income, medium spending  
  - Cluster 1 → High income, high spending (premium customers)  
  - Cluster 2 → Low income, high spending  
  - Cluster 3 → Low income, low spending  
  - Cluster 4 → High income, low spending  

# Tools & Libraries
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  

# Conclusion
K-Means clustering successfully grouped customers into 5 distinct clusters. These insights can support targeted marketing strategies — focusing on Cluster 1 (high spenders) while engaging Cluster 4 (high income but low spending).  
