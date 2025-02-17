# K-Nearest Neighbors (KNN) Classification for Diabetes Prediction

## Overview

This project applies the K-Nearest Neighbors (KNN) algorithm to classify individuals as diabetic or non-diabetic based on medical attributes. The dataset is preprocessed, explored, and evaluated using various performance metrics, including accuracy, confusion matrix, and ROC curve.

## Workflow

1. Data Loading and Preprocessing
The dataset (diabetes.csv) is loaded using pandas.
Missing values in key medical features (Glucose, BloodPressure, SkinThickness, Insulin, BMI) are replaced using mean and median imputation.
The dataset is standardized using StandardScaler to ensure all features contribute equally to model training.
2. Exploratory Data Analysis (EDA)
Distribution Analysis: Histograms and bar charts visualize feature distributions before and after cleaning.
Pair Plots: Display relationships between features and the Outcome variable.
Heatmaps: Identify correlations between different features.
3. Splitting Data for Training and Testing
The dataset is split into training (67%) and testing (33%) subsets using Stratified Sampling to maintain class balance.
4. K-Nearest Neighbors (KNN) Model Training
The Elbow Method is used to determine the optimal number of neighbors (k).
The model is trained with different values of k, and accuracy scores for both training and testing sets are recorded.
A line plot is generated to visualize training vs. testing accuracy for different values of k.
5. Model Evaluation
Confusion Matrix: Displays correct and incorrect predictions.
Classification Report: Shows precision, recall, and F1-score for each class.
ROC Curve: Evaluates the model’s ability to distinguish between diabetic and non-diabetic patients.
6. Decision Boundary Visualization
A decision region plot is generated to visualize how KNN classifies different patients.

## Results & Insights
The optimal number of neighbors (k=11) is selected based on the highest test accuracy.
The ROC curve demonstrates the model's classification performance.
The confusion matrix highlights areas where misclassification occurs.
The model performs well but could be improved by feature engineering or alternative classifiers.

## Technologies Used
Python (for data processing and model building)
pandas, NumPy (for data manipulation)
matplotlib, seaborn (for visualization)
scikit-learn (for model training and evaluation)
mlxtend (for decision boundary visualization)
