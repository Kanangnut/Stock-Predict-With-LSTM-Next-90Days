<b>Stock Price Prediction of Tesla Inc Stock by Long Short-Term Memory (LSTM)</b><br>
This project using TSLA stock from 2010 to 2023

<b>Dataset:</b><br>
The dataset is taken from yahoo website in CSV format.The dataset consists of Open, High, Low, Close, Adj Close Prices and Valume of Tesla Inc.<br>
stocks from 29th Jun 2010 to 19th Junly 2023, all 3286 rows.<br>

<b>Indicator:</b><br>
Stock traders mainly use OHLC (Open, High, Low, Close) for prediction.<br>

<b>Processing</b><br>

Start to transform training and test data in the from of previous day’s that used to predict the next day’s data, following function with step_size = 1. 
And to reshape the data to input for the LSTM model. In this case 2 stacked LSTM layers. to run in a mean squared error (MSE) and training by Adam algorithm. 

MSE = 1/n * Σ(actual value - predicted value)²
Where:  n is the total number of observations
        Σ denotes the sum of the differences
        The difference is squared to eliminate any negative values and emphasize larger differences.
