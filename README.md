#  Wine Dataset Clustering Analysis

##  Overview
This project evaluates three clustering algorithms with different pre-processing methods and evaluation metrics on the Wine dataset to determine which method produces the most effective and meaningful clusters.

##  Algorithms Compared
- **KMeans Clustering**
- **Hierarchical Clustering**
- **MeanShift Clustering**

## Pre-processing Methods used
- **Normalization**
- **Transformation**
- **PCA**
- **Normalization + Transformation**
- **Normalization + Transformation + PCA**
- **Raw Data**


##  Evaluation Metrics
The performance of each algorithm was measured using the following metrics:

- **Silhouette Score**: Measures how well each object lies within its cluster .
- **Calinski-Harabasz Index**: Ratio of between-cluster dispersion to within-cluster dispersion .
- **Davies-Bouldin Index**: Average similarity between each cluster and its most similar one .

##  Results Summary

| Algorithm     | Best Silhouette | Best Calinski-Harabasz | Best Davies-Bouldin |
|---------------|------------------|---------------------------|-----------------------|
| **KMeans**       | 0.5735           | **745.20**                  | **0.4820**              |
| Hierarchical     | 0.5656           | 685.29                      | 0.5343                  |
| MeanShift        | **0.5754**       | 454.06                      | 0.5562                  |

> **Conclusion**: KMeans showed the most consistent and optimal performance across all metrics, making it the best clustering algorithm for this data
>  PCA showed the best pre-processing results for all the algorithms
>  Best cluster-size = 5

## Technologies Used
- Python (Pandas, NumPy)
- Scikit-learn
- Matplotlib / Seaborn (if visualizations are included)

##  File Structure
- `wine_clustering_results.csv`: Tabulated clustering scores
-  `Clustering_assignment.ipynb`: Scripts used for analysis
  

