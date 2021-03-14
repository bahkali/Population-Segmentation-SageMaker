# Population Segmentation

Analy at a portion of US census data and, using a combination of unsupervised learning methods, extract meaningful components from that data and group regions by similar census-recorded characteristics. This case study will be a deep dive into Principal Components Analysis (PCA) and K-Means clustering methods, and the end result will be groupings that are used to inform things like localized marketing campaigns and voter campaign strategies. 

### SageMaker 

Using SageMaker notebook instance to load in and process data, employing unsupervised learning technique
to group data

## K-Mean Clustering

This algorithm that separates an image into segments by clustering data points that have similars traits.
K =  number of clusters(segment)

1. Choose K random center points
2. Assign every data point to a cluster, based on its nearest center point
3. Takes the mean of all the values in each cluster( these mean values become the new center points)
4. repeats steps 2 and 3 until convergence is reached.

You select k, a predetermined number of clusters that you want to form. Then k points (centroids for k clusters) are selected at random locations in feature space.
For each point in your training dataset:

1. You find the centroid that the point is closest to

2. And assign that point to that cluster

3. Then, for each cluster centroid, you move that point such that it is in the center of all the points that are were assigned to that cluster in step 2.

4. Repeat steps 2 and 3 until you’ve either reached convergence and points no longer change cluster membership _or_ until some specified number of iterations have been reached.

## Principal Component Analysis (PCA)

This algorithm reduce the number of features within dataset while retaining the principal components defined as weighted combinations of existing feautures. (Dimensionality Reduction)

Commonly used when you have data with many many features.