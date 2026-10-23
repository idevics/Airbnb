# Airbnb Price Prediction & Superhost Classification

This project analyzes Airbnb listings in London using machine learning.

It focuses on two main tasks:

- Price Prediction: Predicting nightly listing prices.
- Superhost Classification: Predicting whether a host is a Superhost.

## Features

- Data exploration and visualization
- Missing value analysis
- Price distribution analysis
- Outlier detection using IQR, Z-score, and Isolation Forest
- Data preprocessing and feature engineering
- Training and comparing machine learning models
- Model evaluation and feature importance analysis

## Models

### Price Prediction

- Linear Regression
- Ridge Regression
- Decision Tree Regressor
- Random Forest Regressor
- Kernel Ridge Regression

### Superhost Classification

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Classifier (SVC)

## Sampling for Computational Efficiency

Due to their high computational cost, two models were trained using a sample of the training data:

- **SVC (RBF):** Trained on up to 5,000 randomly selected training samples.
- **Kernel Ridge Regression (RBF):** Trained on up to 2,000 randomly selected training samples.

Sampling was used to reduce training time and computational requirements.

**Note:** These models were trained on subsets of the training data rather than the full training sets. Therefore, their results should be interpreted with this limitation in mind when comparing them with other models.

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Dataset

The project uses Airbnb listing data for London from "Inside Airbnb" (https://insideairbnb.com/).

The dataset is downloaded automatically when the notebook runs.

## Evaluation Metrics

Regression:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

Classification:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

## Project Goals

The goal is to explore Airbnb listing data, identify important factors related to nightly prices, compare machine learning models, and classify hosts based on their Superhost status.
