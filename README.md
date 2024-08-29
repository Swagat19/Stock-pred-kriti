# Stock-Market-Prediction
## Problem Statement

The Problem Statement involved building a Stock Price Prediction Model with any Machine Learning and Deep
Learning Techniques trained on 10 years daily price data. Daily Open, High, Low, Close Data will be provided by us from 2013 to 2023  to predict the closing stock price of the future dates in the test set, the training data set had the daily price data of 4 unknown companies from the years 2013 to 2023.

## Exploratory Data Analysis

The EDA consisted of plotting the daily stock prices for observing any trends in the training data. <br>
<br>
<img width="1058" alt="Screenshot 2023-03-29 163347" src="https://user-images.githubusercontent.com/95123465/228514544-ce2996f6-cd2e-4251-b5af-d47ae553789b.png">
<br>
<img width="1053" alt="Screenshot 2023-03-29 163739" src="https://user-images.githubusercontent.com/95123465/228515210-92ebd10a-6b5f-4bcd-83d2-3e9a93135a7e.png">
## Key Observations
<ol>
<li> The variation in the values of the opening, closing, high and low values of stock prices was low </li>
<li>A significant resemblance between the adjusted close and the close prices was observed> The mean difference was almost zero for companies 2,3 and 4 and standard deviation of difference was less than 1.</li>
<li>The stock prices at the end of a quarter varied significantly as compared to their values during the quarter.</li>
</ol>

## Feature Selection

One of the most important aspects of devising a model for any machine learning based task is Feature Selection and Engineering based on the Exploratory Data Analysis.

1. High - Low : Gives information about the volatility of the stock price on a particular day.
2. Quarter End Flag : Stock prices tend to fluctuate more towards the end of a quarter.
3. Volume : Clear indicator of the activity of the stock price on a particular day.
4. Adjusted Close: EDA cleared demonstrated a strong correlation between the closing price and the adjusted close price.
5. Exponential Moving Average (EMA) of Adjusted Close: Moving averages are often good financial indicators for predicting future stock prices.
