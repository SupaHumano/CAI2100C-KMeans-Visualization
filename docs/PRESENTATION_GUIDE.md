# Oral presentation guide

**Juan Luna Santibanez | CAI2100C | Professor Beth Muturi**

## What problem did you solve?

I used K-Means to visualize how the same 150 Iris flowers are grouped when the requested number of clusters changes to four, five and nine.

## What are the model's inputs?

Four numeric measurements: sepal length, sepal width, petal length and petal width. I did not provide the species names during fitting because K-Means is unsupervised.

## What is a cluster?

A group of observations that the algorithm places near the same mathematical center. A cluster is not automatically a biological species.

## What is a centroid?

The average position of a cluster's observations in four-dimensional measurement space. A cross on the chart represents the centroid projected onto the two visible axes.

## What changes from K = 4 to K = 9?

The model uses more centers and divides the same observations into smaller groups. The within-cluster squared distance, or inertia, decreases. That does not imply the existence of nine Iris species.

## What does the elbow chart mean?

It compares inertia against different K values. A change in the rate of improvement can suggest a practical cluster count. It is not definitive proof of the correct number of groups.

## Why is the figure two-dimensional?

A flat screen shows two measurements at once, while the fitted model uses four. The chart is a projection for visualization.

## How did you check the results?

I checked the observation count, the number of centroids, the cluster membership counts and the reproducibility settings for each K.

## Short conclusion

K-Means does not discover species names. It organizes the measurements into the number of clusters requested. Different choices of K change the representation, so the result must be interpreted in context.
