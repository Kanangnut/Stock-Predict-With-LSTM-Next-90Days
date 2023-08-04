<b>Stock Price Prediction of Tesla Inc Stock for Next 90 days using Long Short-Term Memory (LSTM)</b><br>
This project using TSLA stock from 2010 to 2023.

<b>Dataset:</b><br>
The dataset is taken from yahoo website in CSV format.The dataset consists of Open, High, Low, Close, Adj Close Prices and Valume of Tesla Inc. stocks from 29th Jun 2010 to 19th Junly 2023, all 3286 rows.<br>

<b>Indicator:</b><br>
Stock traders mainly use OHLC (Open, High, Low, Close) for prediction.<br>

<b>Processing</b><br>
Start to transform training and test data in the from of previous day’s that used to predict the next day’s data, following function with step_size = 1.
And to reshape the data to input for the LSTM model. In this case 2 stacked LSTM layers. to run in a mean squared error (MSE) and training by Adam algorithm. <br>

![image](https://github.com/Kanangnut/stock-predict-with-LSTM-for-next-3-month/assets/130201193/2490abbf-71c6-4952-9785-f2b1d1cc5c29)



Finally, we plot the Original OHCL dataset with Forecast OHCL values, orange line show forecast values of the next 3 month.<br>
![image](https://github.com/Kanangnut/stock-predict-with-LSTM-for-next-3-month/assets/130201193/b298300c-01e7-4a9c-9144-a528fa3e8335)




