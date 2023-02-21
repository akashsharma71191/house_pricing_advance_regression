# Bike Sharing Model - Linear Regression

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

## General Information

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below. The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not. The company wants to know the following things about the prospective properties:

- Which variables are significant in predicting the price of a house, and how well those variables describe the price of a house.
- Also, determine the optimal value of lambda for ridge and lasso regression.

- Business Goal :
	- Build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.
	- Determine the optimal value of lambda for ridge and lasso regression.
	- This model will then be used by the management to understand how exactly the prices vary with the variables
	- They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns.
	- The model will be a good way for the management to understand the pricing dynamics of a new market.

- The solution is divided into the following sections:

	- Data understanding
	- Data clean up
	- EDA
	- Data preparation
	- Model building and evaluation
	- Observation and inference

## Conclusions
Though the model performance by Ridge Regression was better in terms of R2 values of Train and Test,
it is better to use Lasso, since it brings and assigns a zero value to insignificant features, enabling us to choose
the predictive variables.
It is always advisable to use simple yet robust model.

- The optimal lambda value in case of Ridge and Lasso is as below:

	- Ridge - 3
	- Lasso - 0.0002
- The Number of features used by the model:

	- Ridge - 100
	- Lasso - 74
- The Mean Squared error in case of Ridge and Lasso are:

	- Ridge - 0.142047
	- Lasso - 0.146804
- The Mean Squared Error of Lasso is slightly higher than that of Ridge
- Also, since Lasso helps in feature reduction (as the coefficient value of one of the feature became 0), Lasso has a better edge over Ridge.

- Hence based on Lasso, the factors that generally affect the price are the Roof Material used, Ground living Area of the house, Slope of the property, Central Air conditioning, Garage Area and quality of Finish, Overall quality and condition of the house, Total basement area in square feet and the Basement finished square feet area

- The variables predicted by Lasso in the above bar chart as significant variables for predicting the price of a house. 

- Advise
	- When the market value of the property is lower than the Predicted Sale Price, company should make the investment.


## Technologies Used
- sklearn
- statsmodels
- matplotlib
- seaborn
- pandas
- numpy

## Contact
Created by Akash Sharma