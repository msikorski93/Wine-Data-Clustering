# Wine-Data-Clustering
The goal of this notebook was to introduce and perform clustering algorithms on white wine dataset. Clustering (or grouping) allows us to identify homogeneous groups and recognize pattens within the data without any ground truth labels.
We developed these clustering models to do the unsupervised learning:
* k-means,
* agglomerative,
* spectral.

We also have proved that dimensionality reduction is an essential tool to make sense of the data in the absence of supervision information and applying PCA method improved the clustering process. Below are listed basic scores achieved for each algorithm:

| Method            | Silhouette | Caliński-<br>Harabasz | Davies-<br>Bouldin | Cluster 0 | Cluster 1 | Cluster 2 |
|-------------------|------------|-----------------------|--------------------|-----------|-----------|-----------|
| **k-Means**       | 0.2116     | 1261.7120             | 1.6024             | 1075      | 1308      | 1578      |
| **Agglomerative** | 0.1812     | 1033.0347             | 1.6782             | 1886      | 1382      | 693       |
| **Spectral**      | 0.2004     | 1204.9508             | 1.6378             | 1229      | 1403      | 1329      |

Based on evaluation metrics in the table, the k-means algorithm performed the best on this dataset.

Reference: https://archive.ics.uci.edu/ml/datasets/wine+quality
