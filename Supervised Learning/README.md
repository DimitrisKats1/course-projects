# Supervised Learning Project

This project provides an end-to-end supervised learning pipeline for a binary classification task, covering all crucial stages of model development and evaluation. Specifically, it includes:

## Data Exploration and Preprocessing:
- Initial exploration of dataset characteristics.
- Handling of missing values through median and mode imputation.
- Feature selection and creation (feature engineering).
- Data scaling and encoding of categorical variables using RobustScaler and ColumnTransformer pipelines.

## Model Training and Comparison:
- Split data into training and validation sets.
- Train multiple classification algorithms including Logistic Regression, Random Forest, Support Vector Machines (SVC), K-Nearest Neighbors (KNN), Decision Trees, Naive Bayes, and Neural Networks.
- Compare performance across models using metrics such as accuracy, precision, recall, and F1-score.

## Hyperparameter Tuning and Optimization:
- Apply Grid Search to optimize hyperparameters for selected models.
- Identify the best-performing model based on F1-score and accuracy metrics (Neural Network achieved highest performance).

## Final Model and Prediction:
- Retrain the optimized model on the full training dataset.
- Apply the trained model to make predictions on unseen test data.

This notebook illustrates best practices in supervised learning, highlighting effective preprocessing strategies, model selection, and rigorous evaluation methods.
