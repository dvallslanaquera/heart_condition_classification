# Project 2: Heart Condition classificatory prediction model 
In this notebook we will be exploring the Ames Housing dataset, compiled by Dean De Cock for education purposes and available on Kaggle. The aim of this notebook is to build a predictive model based on the 79 explanatory variables to forecast the final price of a set of around 3000 houses located in Ames, Iowa (USA). 

![](https://github.com/dvallslanaquera/python_projects/blob/master/images/housesbanner.png)

The dataset contains both numerical and categorical features. Most of the features present missing values and are messy, so first of all we are going to do some clean-up so we can build our predictive models on the features without problem. 

Some of the strong points I would highlight about this analysis are:
* Thorough preprocess steps explained with detail were we managed to clean all missing values, outliers and skewness using cutting-edge techniques such as Yeo-Johnson Power Transformation.
![](https://github.com/dvallslanaquera/python_projects/blob/master/images/output_28_0.png)
* Feature selection process included using Recursive Feature Elimination (RFE)
![](https://github.com/dvallslanaquera/python_projects/blob/master/images/output_30_0.png)
* **Stacked predictive model** with prompts the average of three tunned models: XGBoots, LightGBM and Gradient Booster.
* Final **RMSE of 0.1139** (std = 0.0053). The result has been cross-validated with a 10-fold Cross Validation algorithm.  

Some of the notebooks I've used as bibliography for this work were:
1. [A study on Regression applied to the Ames dataset](https://www.kaggle.com/juliencs/a-study-on-regression-applied-to-the-ames-dataset) by Pedro Marcelino 
2. [Regularized Linear Models](https://www.kaggle.com/apapiu/regularized-linear-models) by Alexandru Papiu 
3. [Stacked Regressions to predict House Prices](https://www.kaggle.com/serigne/stacked-regressions-top-4-on-leaderboard/notebook) by Serigne 
