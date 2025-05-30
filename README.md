# Clustering Analysis – Jain & R15 Datasets

This project compares clustering algorithms on two classic datasets: **Jain** and **R15**. We implement and evaluate several unsupervised learning techniques using R.

---

## Datasets

- **Jain**: 2D, 373 points, 2 clusters. [SIPU Datasets](https://cs.joensuu.fi/sipu/datasets/)
- **R15**: 2D, 600 points, 15 clusters. [SIPU Datasets](https://cs.joensuu.fi/sipu/datasets/)

---

##  Methods Used

| Method         | Jain       | R15        | Notes                                   |
|----------------|------------|------------|-----------------------------------------|
| Manual K-means | ✅          | ✅          | From scratch, iterative convergence     |
| K-means + PCA  | ✅          | ✅          | PCA for denoising                       |
| EM (GMM)       | ✅          | ✅          | Probabilistic, soft clustering          |
| DBSCAN         | ✅          | ✅          | Density-based, good for arbitrary shape |
| K-medoids      | ✅          | ✅          | Less sensitive to outliers              |
| Hierarchical   | ✅          | ✅          | Agglomerative, complete linkage         |

---

##  Metrics Used

- Accuracy (when labels available)
- ARI (Adjusted Rand Index)
- NMI (Normalized Mutual Information)
- Silhouette Score
- Sensitivity & Specificity (for 2-cluster case)

---

##  Key Insights

- **K-means + PCA** improves clustering for Jain.
- **GMM** best models elliptical and overlapping clusters.
- **DBSCAN** works well for R15 (clearly separated clusters).
- **K-medoids** and **Hierarchical** are robust and interpretable.

---

##  Libraries

- `ggplot2`, `cluster`, `mclust`, `factoextra`, `dbscan`, `clue`, `aricode`, `clusterCrit`, `caret`

---

##  Author

Bamdad Booyeh 
Course: *Data Mining - Spring 2025*
