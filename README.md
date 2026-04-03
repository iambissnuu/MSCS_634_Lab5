MSCS 634 - Lab 5  
Clustering using Hierarchical and DBSCAN Algorithms  

Overview  
This lab focuses on applying clustering techniques using Hierarchical Clustering and DBSCAN on the Wine dataset from sklearn. The objective is to analyze how different clustering algorithms group data, understand the impact of parameter selection, and evaluate clustering performance using appropriate metrics and visualizations.  

Methods Used  
- Agglomerative Hierarchical Clustering  
- DBSCAN Clustering  
- Data Standardization using StandardScaler  
- Principal Component Analysis (PCA) for visualization  

Evaluation Metrics  
- Silhouette Score (measures cluster separation)  
- Homogeneity Score (measures cluster purity)  
- Completeness Score (measures how well all members of a class are assigned to the same cluster)  

Key Insights  
- Hierarchical clustering produced well-defined clusters, especially when n_clusters = 3, which aligns with the inherent structure of the Wine dataset.  
- The dendrogram provided clear insight into hierarchical relationships between data points.  
- DBSCAN successfully identified noise points (outliers) without requiring a predefined number of clusters.  
- DBSCAN performance was highly sensitive to parameter selection, particularly the eps value.  
- Hierarchical clustering achieved better cluster separation compared to DBSCAN for this dataset.  

Challenges and Decisions  
- Selecting optimal parameters for DBSCAN (eps and min_samples) required experimentation to balance cluster formation and noise detection.  
- Handling noise points affected evaluation metrics such as the silhouette score.  
- PCA was used to reduce dimensionality for visualization, as the dataset contains multiple features.  
- The choice of n_clusters = 3 in hierarchical clustering was based on both dendrogram analysis and evaluation metrics.  

Repository Contents  
- Lab5_Clustering.ipynb (Jupyter Notebook containing implementation and analysis)  
- README.md (Project documentation)  
