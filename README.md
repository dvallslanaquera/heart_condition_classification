# Project 2: Heart Condition classificatory prediction model 
In this notebook we will be exploring how to create a classificatory algorithm and how to tune our models to it in an efficient way. We will be using the Heart Attack Prediction dataset available on Kaggle.

![](https://github.com/dvallslanaquera/python_projects/blob/master/images/heart.png)

This database contains 76 attributes, but all published experiments refer to using a subset of 14 of them. In particular, the Cleveland database is the only one that has been used by ML researchers to this date. The target field refers to the presence of heart disease in the patient. It is integer valued 0 = no/less chance of heart attack and 1 = more chance of heart attack

Some highlights of this analysis are:
* Thorough preprocess steps explained with detail were we managed to clean all missing values, outliers and skewness using cutting-edge techniques such as Yeo-Johnson Power Transformation.
* Feature selection process including a Feature Importance plot using XGBoost model. 
![](https://github.com/dvallslanaquera/python_projects/blob/master/images/eta.png)
* Grid search process explained with detail from scratch up to the last step. 
* **Stacked predictive model** with prompts the average of five tunned classificatory models: Logistic Regression, ExtraTrees, Random Forest, KNN and SVC.
* Final **normalized Gini score of 0.854** (std = 0.0071). The result has been cross-validated with a 10-fold Cross Validation algorithm.  
