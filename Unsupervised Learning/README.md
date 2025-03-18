# Unsupervised Clustering & Ensemble Methods Project

This project is divided into two main parts, each showcasing different techniques in data analysis and modeling:

## Wine Dataset Clustering
- **Data Exploration & Preprocessing:**  
  - Perform EDA on the Wine dataset to inspect distributions, detect outliers, and examine feature correlations.
- **Dimensionality Reduction & Clustering:**  
  - Scale the data using RobustScaler.
  - Reduce dimensions with PCA.
  - Apply K-Means and Hierarchical Agglomerative Clustering to identify clusters.
- **Evaluation:**  
  - Determine the optimal number of clusters using the elbow and silhouette methods.
  - Assess clustering quality using metrics such as Adjusted Rand Index, Normalized Mutual Information, and Fowlkes-Mallows Index.

## Breast Cancer Ensemble Classification
- **Data Setup:**  
  - Load and preprocess the Breast Cancer dataset.
- **Model Training & Tuning:**  
  - Train ensemble classifiers including AdaBoost, Gradient Boosting, and XGBoost.
  - Use Grid Search for hyperparameter tuning based on F1 score and accuracy.
  - Select the best model (XGBoost achieved the highest performance) for final predictions.

This project demonstrates a full workflow from data exploration and preprocessing to model evaluation, applying both unsupervised clustering and ensemble classification techniques.
