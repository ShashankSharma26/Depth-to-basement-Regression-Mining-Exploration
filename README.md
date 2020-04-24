# Depth-to-basement-Regression-Mining-Exploration

The purpose of this project is to build a machine learning regression model to predict the depth to the Iron Ore Copper Gold (IOCG) deposit basements in the South Australia. Geophysics is crucial in understanding what is underneath the ground as as different rocks have different gravity and magnetic sognatures. Hence, Geophysical predictors sourced from the SARIG, the SA government website for geology data (​https://map.sarig.sa.gov.au/​) are used along with the location and depth of historical drillholes to build this regression model.



# Dataset

![](images/dataset%20head.png)

All the predictors are aggregated over different kilometer ranges and different statistical functions so it had an impact on the dimesionality of the data. The dataset used for this project consists of 559 variables and 1777 observations. Therefore, implementing proper feature reduction method is an important aspect of this project to avoid overfitting. 

# Approach

My approach to this project is breifly explained in chronological order below:

* <b>Data cleaning and exploration:</b> Removing the outliers and preparing the dataset for analysis by coverting categorical variables to continuous variables. Understanding the data and finding collinearities within features. 
* <b>Feature reduction:</b> The features that ar highly correlated or add no value to predicting the target variable are removed. Recursive feature elimination method with cross-validation (RFECV) and Pearson correlation are used to perform feature reduction.
* <b>Modelling using Grid Search cross validation for parameter optimisation:</b> Random forest regressor is used to fit a regression line to predict the target variable with the selected features. Grid Search cross validation is used to find the optimal set of parameters for the model.
* <b>Understanding the model:</b> SHAP values are used to observe the importance of each feature in the model.
* <b>Final Model:</b> 5 most important features in the model are used to build a new optimized and efficient model.


Kindly view the jupyter notebook for in-depth explanation of each the above mentioned tasks.  
