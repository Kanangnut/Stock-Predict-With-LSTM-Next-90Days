<b>Stock Price Prediction of Tesla Inc Stock for Next 90 days using Long Short-Term Memory (LSTM)</b><br>
This project using LSTM Recurrent Neural Network for prediction of TSLA stock.

<b>Dataset:</b><br>
The dataset is taken from yahoo website in CSV format.The dataset consists of Open, High, Low, Close, Adj Close Prices and Valume of Tesla Inc. stocks from 29th Jun 2010 to 19th Junly 2023.<br>

<b>Indicator:</b><br>
Stock traders mainly use OHLC average for prediction.<br>

<b>Processing and Model</b><br>
After converting dataset into OHLC average, this has been convert into column of time series data. Then transform to training and test data in the form of previous days. And  input on LSTM model. Following 2 stacked LSTM layers with 1 dense layer, 3 sequences and calculate training and testing Root Mean Square Error (RMSE).


<b>Model</b><br>
![image](https://github.com/Kanangnut/stock-predict-with-LSTM-for-next-3-month/assets/130201193/2490abbf-71c6-4952-9785-f2b1d1cc5c29)


Finally, we plot the Original OHCL dataset with Forecast OHCL values, orange line show forecast values of the next 3 month.<br>
![image](https://github.com/Kanangnut/stock-predict-with-LSTM-for-next-3-month/assets/130201193/b298300c-01e7-4a9c-9144-a528fa3e8335)




