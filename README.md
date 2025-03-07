Clustering Comparison: DBSCAN vs. k-Means vs. Hierarchical Clustering

Overview:
This project demonstrates the performance of various clustering algorithms, focusing on DBSCAN, k-Means, and Hierarchical Clustering. It uses synthetic datasets from scikitlearn, including Moons, Blobs, Circles, and Hierarchical to evaluate how well these algorithms perform under different conditions. The goal is to compare clustering results and identify the strengths and weaknesses of each algorithm for specific types of data.

Datasets Used:
1. Moons Dataset
Description: A two-class dataset with crescent moon-shaped clusters.

2. Blobs Dataset
Description: A simple dataset of well-separated, isotropic Gaussian blobs.

3. Circles Dataset
Description: A dataset consisting of two circles with different radii, with some noise.

Clustering Algorithms:
1. DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
Description: A density-based clustering algorithm that groups together points that are closely packed and labels points in low-density regions as noise.
Strengths:
Works well with noise and outliers
Can find arbitrarily shaped clusters
Weaknesses:
Performance depends on the choice of parameters (Epsloin and min_samples)
Struggles with clusters of varying densities

2. k-Means
Description: A centroid-based clustering algorithm that splits data into clusters by minimizing the within cluster variance.
Strengths:
Fast and simple
Works well with spherical and well-separated clusters
Weaknesses:
Sensitive to the initial choice of centroids
Assumes clusters are spherical and equally sized

3. Hierarchical Clustering
Description: A tree-based clustering algorithm that builds a hierarchy of clusters by either merging smaller clusters or splitting larger clusters.
Strengths:
Specifying number of clusters beforehand is not needed 
Weaknesses:
Computationally expensive for large datasets
Can struggle with clusters of varying densities


Clustering on Synthetic Datasets:

The datasets (Moons, Blobs, Circles, and Hierarchical) were generated using scikit-learn's make_moons, make_blobs, make_circles, and make_h_samples functions.
Each dataset was used to demonstrate the clustering performance of DBSCAN, k-Means, and Hierarchical Clustering.

Clustering Evaluation:

The clustering results were visualized in 2D space using scatter plots. The points were color-coded according to the assigned cluster labels to facilitate comparison.
The plot function plot_clusters() was used to visualize the clusters with distinct colors for each label, which helps in understanding how well each algorithm clusters the data.
Parameter Tuning:


Example Visualizations:<img width="638" alt="Screenshot 2025-03-07 at 4 04 22 PM" src="https://github.com/user-attachments/assets/454765d3-9a0b-48a0-9699-8cc83ffdb440" />

