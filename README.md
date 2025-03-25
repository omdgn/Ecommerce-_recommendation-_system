# Ecommerce-_recommendation-_system


Product Recommendation System

This is a simple machine learning project where I tried to predict whether a product should be recommended to a customer based on their shopping behavior. The idea is to help e-commerce platforms provide more relevant suggestions to users by analyzing previous purchases, product ratings, and spending habits.

Objective:
The goal was to build a classification model that can label a transaction as “Recommended” or “Not Recommended”, depending on a set of rules and features from a customer dataset.

Dataset:
Source: Kaggle – [Customer Shopping Trends](https://www.kaggle.com/datasets/iamsouravbanerjee/customer-shopping-trends-dataset)
Total records: ~3900

Key columns used:
-Previous Purchases
-Review Rating
-Purchase Amount (USD)
-Subscription Status

Other: Season, Category, Item Purchased, Frequency of Purchases, etc.

What I Did?

Preprocessed the data:
Applied one-hot encoding to categorical features.
Scaled numerical values with MinMaxScaler.

Created a new label based on:
-Review Rating > 3
-Previous Purchases > 10
-Purchase Amount > $50

Trained three classification models:
-Logistic Regression
-SVM (RBF kernel)
-k-Nearest Neighbors (k=3)

Evaluated models with metrics:
-Accuracy, Precision, Recall, F1 Score

Results (Test Set):
Model	                Accuracy	  F1 Score
Logistic Regression	  % 82.56	    % 75.63
SVM	                  % 86.28	    % 81.06
KNN (k=3)	            % 63.33 	  % 52.01

SVM performed best and would be the preferred model in a real deployment.

Notes:
Feature engineering took time, especially deciding the rule-based label.
Dataset is relatively small, but sufficient to test basic ML pipelines.
No deep learning or collaborative filtering was used — this is a classical ML approach.

Tools Used:
-Python (pandas, scikit-learn)
-Google Colab


