# Predicting Sleep Quality with Machine Learning

## Overview

This project aims to predict the sleep quality of individuals based on various factors using machine learning techniques. Sleep quality is influenced by a multitude of factors such as age, gender, occupation, sleep duration, physical activity level, stress level, BMI category, heart rate, daily steps, and blood pressure. The dataset used in this project was sourced from Kaggle and underwent thorough data cleaning, exploratory data analysis (EDA), and model training.

## Dataset

The dataset originally obtained from Kaggle contained information on individuals' sleep quality along with demographic and health-related features. The columns in the dataset included:

- **Gender**
- **Age**
- **Occupation**
- **Sleep Duration**
- **Quality of Sleep**
- **Physical Activity Level**
- **Stress Level**
- **BMI Category**
- **Heart Rate**
- **Daily Steps**
- **Blood Pressure** (initially as a single column, later split into **Systolic** and **Diastolic**)

### Data Cleaning and Preprocessing

In the `data cleaning.ipynb` notebook:
- Data cleaning involved converting data types and addressing inconsistencies.
- Categorical variables were encoded using label encoding for compatibility with machine learning algorithms.
- The `Blood Pressure` column was parsed to create two separate columns, `Systolic` and `Diastolic`.
- Exploratory Data Analysis (EDA) techniques like pie charts and heatmaps were used to visualize relationships between variables and understand their distributions.

The cleaned dataset was exported to `cleaned_sleep_data.csv` for further analysis and model training.

## Model Training

In the `model training.ipynb` notebook:
- Several classification algorithms were trained to predict sleep quality based on the preprocessed dataset.
- Algorithms included:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Gradient Boosting
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)
  - Gaussian Naive Bayes (best performing algorithm)
  - Multinomial Naive Bayes
  - Bernoulli Naive Bayes
  - AdaBoost
  
- Cross-validation techniques were employed to evaluate each model's performance robustly.

## Best Performing Model

The Gaussian Naive Bayes classifier emerged as the best-performing model with an accuracy of 86.88%. This model was selected based on its ability to generalize well to unseen data while maintaining high accuracy.

## Conclusion

This project demonstrates the application of machine learning techniques to predict sleep quality based on various demographic, lifestyle, and health-related factors. By leveraging supervised learning algorithms and thorough data preprocessing, we achieved a robust predictive model that can potentially aid in understanding and improving sleep health outcomes.
