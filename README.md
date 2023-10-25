# MachineLearningRelatedCode
This repository contains all machine learning related code I wrote that is somehow worth saving.

## Table of Contents

- [K-Means Clustering Analysis](#k-means-clustering-analysis)


  
## K-Means Clustering Analysis

The K-mean_and_related_evaluation file provides an implementation of the K-Means clustering algorithm, a popular method to partition a dataset into K distinct, non-overlapping clusters. In addition to the core algorithm, we also provide utilities to evaluate the quality of the clustering, employing methods such as Simplified Silhouette Coefficient and Within-Cluster Sum of Squares (WSS).

### Features

- **K-Means Clustering:** Partition your data into a specified number of clusters.
- **Simplified Silhouette Coefficient:** Evaluate the consistency within clusters of data, judging the relative closeness of the data points in different clusters.
- **Within-Cluster Sum of Squares (WSS):** Assess the homogeneity within a single cluster, quantifying how close the data points are within the same cluster.


### Evaluation Metrics

#### Simplified Silhouette Coefficient

This metric calculates the mean intra-cluster distance between each point and the other points in the same cluster. It compares it with the mean nearest-cluster distance - that is, for each sample, the average distance from the other clusters to which the point is not assigned. The coefficient can take values between -1 and 1, where a high value indicates that the object is well matched within its own cluster and poorly matched to neighboring clusters. Since in simplified silhouette we sum the silhouette for every data point, it will take values between -#_of_data and #_of_data.

#### Within-Cluster Sum of Squares (WSS)

WSS measures the compactness of the clustering and we want it to be as small as possible. The idea is to minimize the sum of the squared distances between each member of the cluster and its centroid.

