# Traffic Speed Estimation

## Description
The dataset provides the average traffic speed per hour for a major road in Hong Kong from 2017 to 2018. Part of the dataset is provided as the training data, and your task is to predict the rest. 80% of the dataset is provided as the training data and 20% as the testing data, including the timestamp and the corresponding average speed. We sampled the testing data only from the year 2018 to provide you a training dataset that has the complete data spanning the year 2017. However, the speed information is sometimes missing due to device malfunction.

The task is to submit the predicted results of these testing samples, which are then compared with the ground truth to evaluate the performance of the model.

## Dependencies
```
pip install numpy, pandas, time, datetime, xgboost, plot_importance, plot_tree, pandas_profiling, sklearn, holidays
```

## Methodology
1. Transform to datatime object
2. Split datatime into different categorical data eg. Data, hour
3. Add is holidays or not
4. Using xgboost with GridSearchCV
5. Fit test data to the fitted model
