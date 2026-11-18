# Breast Cancer Classification Using KNN

## Project Overview

This project focuses on classifying breast cancer tumors into two categories: **Malignant (Cancerous)** and **Benign (Non-Cancerous)** using the K-Nearest Neighbors (KNN) classification algorithm.

The project uses the Breast Cancer Wisconsin dataset from Scikit-learn. It involves Exploratory Data Analysis (EDA), data preprocessing, feature scaling, model training, prediction, and performance evaluation.

## Project Objective

- Explore and understand the breast cancer dataset.
- Analyze tumor-related numerical features.
- Perform data preprocessing and feature scaling.
- Implement the K-Nearest Neighbors classification algorithm.
- Compare different distance metrics.
- Evaluate model performance using classification metrics.

## Dataset Information

**Dataset:** Breast Cancer Wisconsin Dataset

**Source:** Scikit-learn (`load_breast_cancer`)

- Total Records: 569
- Total Features: 30
- Target Variable: Cancer Classification

**Target Classes:**

- 0 – Malignant
- 1 – Benign

### Features

The dataset contains numerical measurements related to:

- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Concave Points
- Symmetry
- Fractal Dimension

These measurements include mean, error, and worst-value features.

## Technologies and Libraries Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. Imported the required Python libraries.
2. Loaded the Breast Cancer Wisconsin dataset.
3. Converted the dataset into a Pandas DataFrame.
4. Explored the dataset and target classes.
5. Visualized the relationship between Mean Radius and Mean Texture using a scatter plot.
6. Separated independent and dependent variables.
7. Split the dataset into training and testing sets (80:20).
8. Applied StandardScaler for feature scaling.
9. Implemented the KNN classification algorithm with 3 nearest neighbors.
10. Trained the model and predicted test data.
11. Compared actual and predicted values.
12. Evaluated model performance using different metrics.
13. Compared different distance metrics used in KNN.

## Algorithm Used

### K-Nearest Neighbors (KNN)

KNN is a supervised machine learning algorithm used for classification and regression.

In this project, KNN classifies a tumor based on the majority class among its 3 nearest neighboring data points.

### Distance Metrics Compared

Different distance metrics were implemented to understand their impact on classification accuracy.

| Distance Metric            | Accuracy |
| -------------------------- | -------: |
| Euclidean (Minkowski, p=2) |   92.98% |
| Manhattan                  |   93.86% |
| Hamming                    |   69.30% |
| Chebyshev                  |   91.23% |

*Note: These comparison models were trained on the original, unscaled features, unlike the main scaled KNN model.*

## Model Evaluation

The main KNN classification model was evaluated using the following metrics:

- Accuracy Score
- Confusion Matrix
- Precision
- Recall
- F1-Score
- ROC-AUC Score

### Model Performance

\<escape> \</escape>

| Evaluation Metric |  Score |
| ----------------- | -----: |
| Accuracy          | 98.25% |
| ROC-AUC           | 98.35% |

### Confusion Matrix

|                  | Predicted Malignant | Predicted Benign |
| ---------------- | ------------------: | ---------------: |
| Actual Malignant |                  40 |                2 |
| Actual Benign    |                   0 |               72 |

## Key Learnings

Through this project, I gained practical experience in:

- Working with real-world healthcare datasets.
- Performing Exploratory Data Analysis.
- Understanding feature scaling and its importance in KNN.
- Implementing KNN classification using Scikit-learn.
- Understanding different distance metrics.
- Evaluating classification models using multiple performance metrics.
- Comparing actual and predicted values.

## Conclusion

This project helped me understand the practical implementation of the K-Nearest Neighbors classification algorithm. By applying data preprocessing, feature scaling, model training, and evaluation techniques, the model achieved an accuracy of 98.25% on the test dataset.
