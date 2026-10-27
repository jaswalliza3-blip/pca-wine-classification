# PCA Wine Classification

## Project Overview

This project demonstrates the use of **Principal Component Analysis (PCA)** for dimensionality reduction and its effect on a machine learning classification problem.

The Wine dataset from Scikit-learn contains 13 chemical features. PCA is applied to transform these features into a smaller set of principal components while retaining as much of the data's variance as possible.

A Logistic Regression classifier is then used to compare classification performance before and after PCA.

## Objective

The main objectives of this project are to:

- Understand the need for dimensionality reduction.
- Standardize features before applying PCA.
- Analyze explained variance.
- Reduce 13 features to 2 principal components for visualization.
- Compare model performance with and without PCA.
- Understand the trade-off between dimensionality reduction and information loss.

## Dataset

The project uses the **Wine dataset** provided by Scikit-learn.

It contains:

- **178 samples**
- **13 numerical features**
- **3 wine classes**

The features represent different chemical properties of the wines.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Principal Component Analysis (PCA)
- Logistic Regression

## Project Workflow

```text
Wine Dataset
     ↓
Data Exploration
     ↓
Train-Test Split
     ↓
Feature Standardization
     ↓
PCA
     ↓
Explained Variance Analysis
     ↓
2D Visualization
     ↓
Logistic Regression
     ↓
Performance Comparison
```

## Why PCA?

When a dataset contains many features, working with all of them can make analysis and visualization more difficult.

PCA creates new variables called **principal components** that are combinations of the original features.

The first principal component captures the greatest possible amount of variance, the second captures the next greatest amount, and so on.

In this project, the original **13 features are reduced to 2 principal components** for visualization.

## Results

Two Logistic Regression models are compared:

1. Logistic Regression using all 13 standardized features.
2. Logistic Regression using only 2 PCA components.

The project evaluates both models using test accuracy and classification reports.

The explained variance analysis is also used to understand how much information is retained by the principal components.

## Key Learnings

Through this project, I learned:

- Why feature scaling is important before PCA.
- How PCA transforms high-dimensional data.
- How explained variance helps determine the number of components.
- How dimensionality reduction can make visualization easier.
- How reducing dimensions can involve a trade-off between simplicity and predictive performance.
- How to avoid data leakage by fitting preprocessing steps only on the training data.

## Project Structure

```text
pca-wine-classification/
│
├── PCA_Wine_Classification_Project.ipynb
└── README.md
```

## Future Improvements

- Experiment with different numbers of principal components.
- Compare PCA with other dimensionality-reduction techniques.
- Test additional classification algorithms.
- Analyze PCA loadings to understand which original features contribute most to each component.
