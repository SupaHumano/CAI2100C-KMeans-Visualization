# Methodology and reproducibility

**Student:** Juan Luna Santibanez  
**Course:** CAI2100C-2267-6908, Machine Learning Foundations  
**Instructor:** Professor Beth Muturi  
**Task:** Assignment 7, K-Means Visualization

## Objective

Use the same Iris observations to visualize **K = 4, K = 5 and K = 9**. K = 3 is a classroom reference only.

## Data

The 150 rows are organized as four measurements followed by a species label. The label is **not** a K-Means input. Missing numeric measurements: zero. Each observation appears once.

## Model controls

All required experiments use scikit-learn KMeans with `init='k-means++'`, `n_init=10`, `max_iter=300` and `random_state=0`. This controls random initialization and makes repeated notebook runs reproducible in the same computational environment.

## Interpretation rules

The fitted model uses **four measurements**. A 2D figure shows a projection of its assigned labels and centroid coordinates into petal-length and petal-width axes. Overlapping dots on a figure can still differ in the other two dimensions. Cluster IDs are arbitrary and do not represent species.

## Internal validation

Check `len(labels) == 150`, `len(centers) == K`, `sum(cluster_sizes) == 150`, numeric and finite centroids, and decreasing inertia as K grows. Results can vary across library versions or initialization settings. Do not treat smaller inertia alone as proof of a better biological grouping.

## Delimitation

This public portfolio is an independent presentation of the specified experiment. It does not reproduce instructor-authored notebook or presentation files. The official assignment remains separate.
