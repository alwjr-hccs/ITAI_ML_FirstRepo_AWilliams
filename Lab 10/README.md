What is the fundamental difference between supervised and unsupervised learning? Supervised learning uses labeled data — the model is trained with input–output pairs and learns to map features to known targets.
Unsupervised learning uses unlabeled data — the model tries to discover structure or patterns on its own, such as clusters or latent components.

In short: Supervised = learn from answers. Unsupervised = discover structure without answers.

In the K-Means elbow plot, why don't we just choose the largest possible k to get the lowest inertia? Because inertia always decreases as k increases — even if the clusters become meaningless.
Choosing a very large k leads to:

Overfitting the noise

Clusters that are too small to be useful

Centroids that don’t represent meaningful customer groups

The elbow method finds the point where adding more clusters gives diminishing returns, balancing simplicity and explanatory power.

In the PCA results, the first two principal components explained over 95% of the variance. What does this tell you about the original 4-dimensional Iris dataset? It tells you that:
Most of the meaningful structure in the data lies in a lower‑dimensional subspace

The original 4 features contain redundancy or correlated information

You can visualize and analyze the dataset effectively in just 2 dimensions without losing much information

In other words, the Iris dataset is highly compressible — its essential structure is almost entirely captured by two principal components.
