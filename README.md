# Stock-price-prediction-using-ExplainableAI

This project focuses on predicting the closing price of a stock based on historical data. Several machine learning algorithms are employed, including Decision Trees, Random Forest, and XGBoost. The models are tuned using grid search or randomized search, and their performance is evaluated using metrics like Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared.

![Decision Tree Visualization](images/decision_tree_plot.png)

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data](#data)
3. [Modeling and Evaluation](#modeling-and-evaluation)
4. [Feature Importance](#feature-importance)
5. [Model Interpretation](#model-interpretation)
6. [Performance Comparison](#performance-comparison)

## Project Overview

The goal of this project is to create a model that predicts the closing price of a stock given certain features such as "Open", "High", "Low", and "Volume". The models are trained on historical data and tested for accuracy and error metrics.

## Data

The dataset used in this project is a CSV file containing historical stock data. The features used for prediction include:
- **Open**: Opening price of the stock
- **High**: Highest price during the day
- **Low**: Lowest price during the day
- **Volume**: Number of shares traded

The target variable is **Close**, representing the closing price of the stock.

## Modeling and Evaluation

Three different models are trained and evaluated:
1. **Decision Tree**: A simple tree-based model.
2. **Random Forest**: An ensemble of decision trees.
3. **XGBoost**: A more complex ensemble method based on gradient boosting.

The models are tuned using grid search or randomized search to find the best parameters. The best model is then used to predict the test set, and the performance is measured using MSE, MAE, and R-squared.

## Feature Importance

Feature importance is analyzed for each model to understand which features contribute most to the predictions. Below are the feature importance plots for each model:

![Feature Importances - Decision Tree](images/feature_importance_decision_tree.png)
![Feature Importances - Random Forest](images/feature_importance_random_forest.png)
![Feature Importances - XGBoost](images/feature_importance_xgboost.png)

## Model Interpretation

To understand the decision-making process of the models, interpretable AI tools like SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-agnostic Explanations) are used. These tools provide insights into how each feature impacts the model's prediction.

![SHAP Summary Plot](images/shap_summary_plot.png)

## Performance Comparison

A performance comparison among the three models was conducted. The comparison includes accuracy, MSE, and MAE metrics.

![Model Accuracy Comparison](images/model_accuracy_comparison.png)
![MSE Comparison](images/mse_comparison.png)
![MAE Comparison](images/mae_comparison.png)

## Conclusion

This project demonstrates how different machine learning models can be used to predict stock prices. By comparing the performance of different models and analyzing feature importance, the project provides valuable insights into the factors influencing stock price predictions. Additionally, the use of interpretable AI tools helps understand the underlying decision-making process of the models.
