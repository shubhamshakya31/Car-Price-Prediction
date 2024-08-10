# Car Price Prediction

## Overview

This project aims to predict the price of used cars based on various features using machine learning techniques. The workflow involves thorough data cleaning, extensive exploratory data analysis (EDA), feature engineering through one-hot encoding, and building a predictive model.

### Problem Statement

The used car market is vast and diverse, with prices varying widely based on multiple factors such as the car's make, model, age, mileage, and more. The goal of this project is to develop a model that accurately predicts the price of a used car, aiding both buyers and sellers in making informed decisions.

## Data Cleaning

Data cleaning was a crucial step to ensure the quality and reliability of the dataset. The raw dataset contained missing values, inconsistencies, and outliers that could adversely affect model performance. The following steps were undertaken:

- **Handling Missing Values**: Addressed missing values by filling them with appropriate statistics (e.g., mean, median) or removing records with too many missing values.
- **Outlier Detection and Removal**: Identified and removed outliers in continuous variables like price and mileage to prevent skewing the model.
- **Standardization**: Corrected formatting issues, such as inconsistent date formats and text data standardization (e.g., "petrol" vs. "Petrol"), to ensure uniformity across the dataset.

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to uncover patterns and relationships within the data. The analysis included:

- **Distribution Analysis**: Examined the distribution of key features such as price, mileage, and year of manufacture to understand their spread and central tendencies.
- **Correlation Analysis**: Utilized a heatmap to visualize correlations between numerical features and the target variable (price), highlighting influential factors.
- **Feature Relationships**: Explored relationships between categorical variables (e.g., fuel type, transmission) and price using scatter plots, box plots, and bar charts.
- **Insights**: Documented key insights, such as depreciation rates and mileage impact on price, to guide feature engineering and model selection.

## Feature Engineering

To prepare the data for modeling, several feature engineering techniques were applied:

- **One-Hot Encoding**: Converted categorical variables such as `Make`, `Model`, `Fuel Type`, and `Transmission` into numerical format using one-hot encoding.
- **Feature Scaling**: Scaled continuous variables like `Mileage` and `Year` to ensure all features contributed equally to the model.
- **Feature Selection**: Dropped irrelevant or redundant features based on EDA insights to reduce noise and improve model performance.

## Model Building

The cleaned and engineered dataset was used to build a machine learning model for predicting car prices. The following steps were followed:

- **Model Selection**: Chose a linear regression model due to its simplicity and effectiveness in regression problems, providing interpretability of feature impact on price.
- **Model Training**: Split the dataset into training and test sets. Trained the model on the training set using the selected features.
- **Model Evaluation**: Evaluated the model's performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared to assess prediction accuracy on unseen data.
- **Hyperparameter Tuning**: Conducted basic hyperparameter tuning to optimize model performance.


