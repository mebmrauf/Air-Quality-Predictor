# Air Quality Predictor

## Overview

Air quality prediction is a critical task in environmental science and public health management. This project aims to classify air quality into categories such as **Good**, **Moderate**, **Poor**, and **Hazardous** based on various environmental factors using machine learning models. The dataset contains attributes such as temperature, humidity, pollutant levels (PM2.5, PM10, NO2, SO2, CO), proximity to industrial areas, and population density, which serve as predictors for the classification task.

The goal is to preprocess the data, scale the features, split the dataset, and train multiple models to identify the most effective one for the classification task. With increasing urbanization and industrial activities, air quality monitoring is essential to ensure public safety and mitigate health risks associated with poor air quality.

---

## Features

- **Dataset Preprocessing**: Cleaning and encoding categorical data.
- **Feature Scaling**: Normalization using `MinMaxScaler`.
- **Dataset Splitting**: Stratified random sampling for unbiased evaluation.
- **Model Training**: Evaluation of Logistic Regression, Naive Bayes, and Random Forest classifiers.
- **Metrics**: Accuracy, precision, recall, and confusion matrix analysis.

---

## Dataset

The dataset contains:

- **Features**: 9 features, including temperature, humidity, pollutant levels, and population density.
- **Samples**: 5,000 samples.
- **Target Variable**: 
  - **Good**, **Moderate**, **Poor**, **Hazardous** (encoded numerically using `LabelEncoder`).
- **Class Distribution**: Slightly unbalanced, with instance counts ranging from 4,577 to 4,641.
- **Source**: [Air Quality Dataset on Kaggle](https://www.kaggle.com/datasets/mujtabamatin/air-quality-and-pollution-assessment).

---

## Models and Performance

Three machine learning models were trained and tested:

1. **Logistic Regression**
   - A statistical model used for binary and multiclass classification tasks, estimating probabilities using a logistic function.

2. **Naive Bayes**
   - A probabilistic classifier based on Bayes' theorem, assuming independence between features.

3. **Random Forest**
   - An ensemble method that builds multiple decision trees and aggregates their predictions for improved accuracy and reduced overfitting.

### Results:
- **Logistic Regression**: 82.53% accuracy.
- **Naive Bayes**: 82.93% accuracy.
- **Random Forest**: 86.13% accuracy.

Detailed analysis was performed using **precision**, **recall**, and **confusion matrices** to evaluate the performance of each model.
