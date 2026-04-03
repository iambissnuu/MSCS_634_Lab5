# MSCS 634 - Lab 5  
## Clustering using Hierarchical and DBSCAN Algorithms  

## Overview  
This lab focuses on applying clustering techniques using Hierarchical Clustering and DBSCAN on the Wine dataset from sklearn. The objective is to analyze how different clustering algorithms group data, understand the impact of parameter selection, and evaluate clustering performance using appropriate metrics and visualizations.  

## Methods Used  
- Agglomerative Hierarchical Clustering  
- DBSCAN Clustering  
- Data Standardization using StandardScaler  
- Principal Component Analysis (PCA) for visualization  

## Evaluation Metrics  
- Silhouette Score – Measures cluster separation  
- Homogeneity Score – Measures cluster purity  
- Completeness Score – Measures how well all members of a class are assigned to the same cluster  

## Key Insights  
- Hierarchical clustering produced well-defined clusters, especially when n_clusters = 3, aligning with the dataset structure.  
- The dendrogram provided insight into hierarchical relationships between data points.  
- DBSCAN identified noise points without requiring a predefined number of clusters.  
- DBSCAN performance was sensitive to parameter selection, particularly eps.  
- Hierarchical clustering achieved better cluster separation compared to DBSCAN for this dataset.  

## Challenges and Decisions  
- Selecting optimal parameters for DBSCAN required experimentation.  
- Noise points affected evaluation metrics such as the silhouette score.  
- PCA was used to reduce dimensionality for visualization.  
- The choice of n_clusters = 3 was based on dendrogram analysis and evaluation metrics.  

## Repository Contents  
- Lab5_Clustering.ipynb – Jupyter Notebook with implementation and analysis  
- README.md – Project documentation  
