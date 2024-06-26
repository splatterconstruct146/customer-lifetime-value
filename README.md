# Customer Lifetime Value
A project that uses the XGBoost Regressor and CLassifier to predict the amount customers will spend in a given time period, and the probability of them spending.

## Motivation
This project was created as an attempt to understand and use XGBoost models in business contexts. 

Some basic questions the project strives to answer:
1. TO understand which customers to focus on.
2. Predict how much customers will likely spend in the future.
3. Predict the probability of customers making a purchase in the future. 

## Shortcomings
Only tested using XGBoost - since that was the main goal. Did not test if other regression and classifier models would work better.

## Summary of dataset
The dataset is based on cdnow's customer transaction records. SPecifically customers who signed-on or made their first purchases udring 1997 Jan 01 to 1997 Mar 25.

A breakdown of the dataset is as follows:
* customer_id: self-explanatory
* date: date of transaction by the customer (represented by their customer_id)
* quantity: quantity of items purchased
* amount: sum amount of the transaction

## Methodology
1. Exploratoy data analysis.
2. Time splitting and feature engineering
   i. Time series data, so needed to split the dates as feature and target.
   ii. XGBoost requires some amount of feature engineering to function well - which is performed in this step.
3. Model training and evaluation
4. Understanding feature importance
5. Saving the models and outputs (csv, and pickle files)
6. Business questions answer attempt

## Future works
Will attempt to create a Dash app/applet that allows users to interact with the dataset. The goal here is if this applet was created for business stakehlders, they would be able to make use of the dataset without needing to touch the code.
