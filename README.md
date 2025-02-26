# Image-Segmentation-DBSCAN
This project demonstrates the application of DBSCAN (Density-Based Spatial Clustering of Applications with Noise) for image segmentation. It segments an image into different regions based on pixel values and their coordinates. 

Requirements
To run the project, you need to install the following Python libraries:

numpy
opencv-python
scikit-learn
matplotlib


Image Loading and Preprocessing: The image is loaded and its pixel values are extracted. The pixel coordinates (x, y) are also created to enable spatial analysis for clustering.

DBSCAN Clustering: DBSCAN is applied on the pixel coordinates and the RGB values of the pixels. The eps and min_samples parameters of DBSCAN determine the sensitivity and size of the clusters.

Silhouette Score for Random Data: The Silhouette Score is computed for the 10% random data points that were added. The silhouette score measures how well the random points (treated as noise) fit the clusters formed by DBSCAN. A high silhouette score for random points indicates that the noise points are well-separated from the clusters.

Result Visualization: The segmented image is displayed with each cluster assigned a random color. Noise points, labeled as -1 by DBSCAN, are treated separately and can be displayed in a unique color.
