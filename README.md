# The data in this dataset is collected from FRED , Factors Affectiong House prices in USA over 20 years
collection of all the dataset 
 link--->   https://fred.stlouisfed.org/ 

 Population data = POPTHM

 GDP data code = GDP

 Mortgage = MORTGAGE30US

 Unemployement rate = U2RATE

 Inflation =FPCPITOTLZGUSA

 price = ASPUS

inconme = MEHOINUSA672N

housing price index = CSUSHPISA

Steps 

1. Data ingestion 
2. Exploratory Data analysis 
3. Feature engineering
4. Model building
5. Predictions


There are several feature Affection the price, from which i have taken the important features.
All the data set with monthly frequencies are grouped by year taking the year mean 



# Linear Regression:
Linear regression is a simple linear approach to modeling the relationship between a dependent variable (target) and one or more independent variables (features).

# Formula:
In simple linear regression with one feature:
y = β0 + β1 * x + ε

# Where:

y is the dependent variable (target).
x is the independent variable (feature).
β0 is the intercept.
β1 is the coefficient for the feature x.
ε is the error term.

# RandomForestRegressor:
Random Forest is an ensemble learning method that combines multiple decision trees to make predictions. It is effective for regression and classification tasks.

# Formula:
Random Forest doesn't have a single formula like linear regression. Instead, it combines the predictions of multiple decision trees. The final prediction is typically the average (for regression) or mode (for classification) of the predictions from individual trees.

# Lasso (Least Absolute Shrinkage and Selection Operator):
Lasso is a linear regression technique that adds a penalty term (L1 regularization) to the linear regression cost function. It encourages feature selection by setting some feature coefficients to exactly zero.

# Formula:
Lasso adds an L1 penalty term to the standard linear regression cost function:
Loss = RSS + α * ∑|βi|

# Where:

Loss is the cost function to be minimized.
RSS is the residual sum of squares (the standard linear regression cost).
α is the regularization parameter (hyperparameter).
βi are the coefficients of the features.


# Ridge Regression:
Ridge regression is another linear regression technique that adds a penalty term (L2 regularization) to the linear regression cost function. It helps prevent multicollinearity and controls overfitting.

# Formula:
Ridge adds an L2 penalty term to the standard linear regression cost function:
Loss = RSS + α * ∑(βi^2)

# Where:

Loss is the cost function to be minimized.
RSS is the residual sum of squares (the standard linear regression cost).
α is the regularization parameter (hyperparameter).
βi are the coefficients of the features.


# ElasticNet:
ElasticNet is a linear regression technique that combines L1 (Lasso) and L2 (Ridge) regularization terms to balance feature selection and multicollinearity control.

# Formula:
ElasticNet combines both L1 and L2 penalties:
Loss = RSS + α * ∑|βi| + β * ∑(βi^2)

# Where:

Loss is the cost function to be minimized.
RSS is the residual sum of squares (the standard linear regression cost).
α and β are the regularization parameters (hyperparameters).
βi are the coefficients of the features.
In practice, these methods are implemented with optimization algorithms to find the optimal coefficients that minimize the cost function, considering the regularization terms. The choice between these methods depends on the specific problem and the balance needed between feature selection and multicollinearity control.





! [Price changes over 20 years](https://github.com/abhigujjar/USA-house-price-prediction/blob/main/image.png)




As it can be seen in this graph, the prices have changed over the year non linear way.
2000's it was around $ 200000
upto 2008 and 2009 mid it has raised linearly around $ 320000, due to ressession in 2009-10 the prices have come down around $ 260000.
After ression the market gained a slow upward move around the year 2014.
We can see the upward move in the market.

