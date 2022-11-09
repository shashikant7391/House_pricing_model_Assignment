# Housing price prediction assignment- Surprise Housing
>Model on prediction of price of houses (Company- 'Surprise housing') with Multiple Linear Regression using Ridge and Lasso.


## Table of Contents
* Step 1: Business Objective
* Step 2: Reading and Understanding the Data, Visualising data
* Step 3: Treating outliers
* Step 4: Splitting the Data into Training and Testing Sets, scaling and derived columns
* Step 5: Building a linear model using Statsmodel OLS to eliminate features based on p values
* Step 6: VIF based feature elimination for multicollinearity
* Step 7: Model building using Ridge and Lasso
* Step 8: Model Evaluation of Ridge and Lasso

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement/General Information

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:
Which variables are significant in predicting the price of a house, and
How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression.


- Business Goal:
You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Ridge regression lambda = 50, R2 score: 0.765
- Top 5 features from Ridge regression are: OverallQual, KitchenQual_TA, Neighborhood_NoRidge, KitchenQual_Gd, BsmtQual_Gd.
 - Lasso regression lambda = 100, R2 score: 0.767
- Top 5 features from Lasso regression are: OverallQual, KitchenQual_TA, KitchenQual_Gd, Neighborhood_NoRidge, BsmtQual_Gd.
- Though there is not much difference between the metrics of obtained model after Ridge and Lasso regression, we prefer to apply Lasso because it has further eliminated the dependent features from the model, by bringing the lesser dependent variables coefficient to zero. Note: We have already taken care of multicollinearity before, by using VIF.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python - version 3.10
- Pandas - version 1.5.0
- Scikit-learn - version 0.20
- Statsmodels - version 0.11

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- This project is part of advanced regression assignment.

## Contact
Created by @ShashiKant7391 - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
