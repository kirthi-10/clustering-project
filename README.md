# clustering-project

The goal of this analysis is to cluster penguin species based on their physical characteristics using Principal Component Analysis (PCA) followed by both K-means clustering.

The dataset contains measurements such as culmen length, culmen depth, flipper length, body mass, and sex of penguins. By applying PCA, we will reduce the dimensionality of the data to focus on the most significant features. We will then use K-means clustering to identify distinct groups of penguins, potentially corresponding to different species or other meaningful classifications.

**1. culmen_length_mm, culmen_depth_mm, flipper_length_mm, and body_mass_g:** All have 342 non-null values out of 344 entries, meaning that each of these columns has 2 missing values. These columns are of the data type float64.

**2. sex:** This column has 335 non-null values out of 344 entries, meaning there are 9 missing values. The data type for this column is object, which means it contains text or categorical data.

**Applying PCA before clustering in our task serves to:**

* **Reduce dimensionality:** Making the data more manageable and highlighting the most important features.
* **Enhance clustering:** By focusing on the most informative components, it improves the accuracy and performance of the clustering algorithm.
* **Enable visualization:** Allowing us to see the potential clusters in a lower-dimensional space.

Thus, PCA is a crucial step that prepares the data for more effective and interpretable clustering.


**K-Means Clustering Process:**

**1. Initialize Centroids:** Randomly select K points as the initial centroids for the clusters.

**2. Assign Data Points:** For each data point, calculate its distance to each centroid and assign it to the nearest centroid's cluster.

**3. Calculate SSE:** Compute the Sum of Squared Errors (SSE), which measures the variance within each cluster. The objective is to minimize this SSE.

**4. Update Centroids:** Recalculate the centroids by determining the mean of the data points in each cluster.

**5. Iterate Until Convergence:** Repeat steps 2 through 4 until the centroids stabilize and no longer change significantly.
