# Weather Temperatue Prediction : Project Overview

* Created a tool that predict apparent temperature **Linear Regression: (RMSE ~ 0.9886 (C)); Decision Tree: (RMSE ~ 0.0676 (C))** of a particular location based off some features gotten from historical data

* Got a Test Accuracy of **Linear Regression: 99.07%; Decision Tree: 99.995%**

* Engineered features by encoding categorical columns and parsing out date

* Used Linear Regression (Least Squares) and Decision Tree Regressor as model

___
### Code and Resources Used
Python Version: 3.8
Packages: pandas, numpy, matplotlib, seaborn, plotly, sklearn
* Packages can be installed by running the notebook
Dataset: [Weather Temperature Dataset](https://www.kaggle.com/budincsevity/szeged-weather "Gotten from Kaggle)

___
### Features
* Formatted Date
* Summary
* Precip Type
* Temperature (C)
* Humidity
* Wind Speed (km/h)
* Wind Bearing (degrees)
* Visibility (km)
* Pressure (millibars)
* Daily Summary

### Target
* Apparent Temperature (C)
___

### Feature Engineering / Data Cleaning
I needed to clean the data to make it useful for out model. I did the following:
* Parsed date out of string
* Imputed the missing values of Precip Type by filling it with the most frequest value
* Removed redundant column with too much unique values
* Hot Encoded category columns so they ca be sutable for our model

___
### Model Building

I split the data into train and test based on the year they were recorded with samples recorded before 2016 as train and samples recorded in 2016 as test data.

I used **Linear Regression (Least Squares) and Decision Trees Regressor** as the algorithm for the model
___

### Model Performance
I used Root Mean Squared Error cause the data had some outliers and it was preferred

The model performed well with the following with the following metrics
* For Linear Regression
    * RMSE - 0.9886
    * Test Accuracy - 99.07%

* For Decision Trees Regressor
    * RMSE - 0.0676
    * Test Accuracy - 99.995%






















