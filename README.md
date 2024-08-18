# XGBoost-time-series-forecasting

## Introduction
Is there a way to predict the unpredictable? While predicting the exact future price of a stock is nearly impossible, this work attempts to shrink the possible spread of future prices into a confidence interval, thereby reducing exposure to market volatility.


**Keywords:** XGBoost, LSTM, Windowing, Feature Engineering, Hyperparameter Tuning, Mean Absolute Error, Predictions.

## Table of Contents
- [Introduction](#introduction)
- [Data](#data)
- [Feature Engineering](#feature-engineering)
- [LSTM-XGBoost](#lstm-xgboost)
- [Alternatives](#alternatives)
- [Conclusion](#conclusion)


## Data
Apple Inc. (AAPL) is the focus of this study due to its high market capitalization and volatility, making it an interesting candidate for technical analysis. The volatility, or standard deviation of stock prices, provides opportunities in trading by increasing potential gains or losses. This analysis, although focused on AAPL, could be adapted for assets with different volatility profiles.

## Feature Engineering
(Include details about the features used in the model, how they were selected, and any transformations applied to the data.)

## LSTM-XGBoost
The core of this project is the hybrid model combining LSTM and XGBoost:

- **LSTM:** Captures temporal dependencies and trends in the stock price data.
- **XGBoost:** Efficiently handles complex patterns and relationships within the data.

This section details the methodology, including how XGBoost's tree-building process is optimized using a Greedy algorithm, the combination of models to minimize error, and the iterative improvement of performance targets.


## Training the Model
Model training involved hyperparameter tuning and window optimization using time series cross-validation. Unlike conventional cross-validation, time series cross-validation ensures that the algorithm respects the temporal order of data, crucial in financial time series. The user-defined GridSearchCV, leveraging `ParameterGrid`, was used to systematically explore combinations of parameters. Considerations were made regarding the computational expense of this approach versus its benefits.

## Alternatives
(Discuss any alternative models or methods considered, and why the chosen hybrid model was selected.)

## Conclusion
This project demonstrates the application of a hybrid LSTM-XGBoost model for stock price prediction. While the results are promising, the model is not fully optimized and should not be relied upon for investment decisions. Further refinement and testing could improve its accuracy and reliability.
"""

