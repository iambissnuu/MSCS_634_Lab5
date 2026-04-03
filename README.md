# MSCS 634 - Lab 5  
## Clustering using Hierarchical and DBSCAN Algorithms  

## Overview  
This lab explores clustering techniques using Hierarchical Clustering and DBSCAN on the Wine dataset. The objective is to analyze clustering performance, evaluate parameter sensitivity, and understand how dataset characteristics influence algorithm effectiveness.  

## Methods Used  
- Agglomerative Hierarchical Clustering  
- DBSCAN Clustering  
- Data Standardization using StandardScaler  
- Principal Component Analysis (PCA) for visualization  

## Evaluation Metrics  
- Silhouette Score – Measures cluster separation  
- Homogeneity Score – Measures cluster purity  
- Completeness Score – Measures how well members of a class are grouped together  

## Key Insights  
- Hierarchical clustering produced well-defined clusters with strong separation, aligning closely with the dataset’s inherent structure.  
- DBSCAN showed high sensitivity to the eps parameter, with smaller values resulting in excessive noise and larger values causing cluster merging.  
- No optimal eps value was found that produced meaningful cluster separation for this dataset.  
- DBSCAN resulted in high completeness but low homogeneity, indicating poor separation between classes despite grouping data points together.  
- The Wine dataset contains compact and well-separated clusters, making it more suitable for distance-based methods rather than density-based approaches.  

## Challenges and Decisions  
- Selecting appropriate eps values for DBSCAN required experimentation due to sensitivity in high-dimensional space.  
- Initial parameter choices resulted in all data points being classified as noise, requiring adjustment of eps values.  
- PCA was used to reduce dimensionality for visualization purposes.  
- The selection of n_clusters = 3 for hierarchical clustering was based on silhouette scores and dendrogram interpretation.  

## Repository Contents  
- Lab5_Clustering.ipynb – Jupyter Notebook with implementation and analysis  
- README.md – Project documentation  
