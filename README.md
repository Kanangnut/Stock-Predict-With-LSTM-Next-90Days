<b>Stock Price Prediction of Tesla Inc Stock for Next 90 days using Long Short-Term Memory (LSTM)</b><br>
This project using LSTM Recurrent Neural Network for prediction of TSLA stock.

<b>Dataset:</b><br>
The dataset is taken from yahoo website in CSV format.The dataset consists of Open, High, Low, Close, Adj Close Prices and Valume of Tesla Inc. stocks from 29th Jun 2010 to 19th July 2023.<br>

<b>Indicator:</b><br>
Stock traders mainly use OHLC average for prediction.<br>

<b>Processing and Model</b><br>
After converting dataset into OHLC average, this has been convert into column of time series data. Then transform to training and test data in the form of previous days. And  input on LSTM model. Following 2 stacked LSTM layers with 1 dense layer, 4 sequences then calculate training and testing Root Mean Square Error (RMSE).

<b>Version</b><br>
Python 3.11.2 and deep learning library Keras and Tensorflow.<br>

The trining and testing of OHLC average price:
![image](https://github.com/Kanangnut/Stock-predict-with-LSTM-for-next-3-month/assets/130201193/e2690e71-f4d1-450a-87c9-8dbe13f335ee)


Finally, we plot the Original OHCL dataset with Forecast OHCL values, orange line show forecast values of the next 3 month.<br>
![image](https://github.com/Kanangnut/Stock-predict-with-LSTM-for-next-3-month/assets/130201193/24096bb2-d1f8-41cc-a05b-09094b7fd073)

<b>Conclusion:</b><br>
Since difference among of the training and testing RMSE are 0.69 and 9.44 respectively, from the testing result quit higher than the training set. It likely this model badly over fit of the data. However stock price from the last day of data set on 19 July 2023 was 294.0275 and using this model and price of next three days are predicted as 307.7730, 261.8300 and 265.2500 - which were 271.1475, 262.955 and 262.2200 on 20th, 21th and 24th July 2023 according to yFinance. From the result accuracy of OHLC of three days show at 95.79%, so the trend of future values of any time period can be predicted usind this model. In my view, this work can help the quantitative traders to take decisions.

<b>Observation:</b><br>
The model's overfitting to the training data is a concern, and it may not perform well on unseen data. However, the predictions are reasonably accurate, suggesting that the model can help predict the trend of future stock prices with a relatively high level of confidence. The model's performance could be beneficial for quantitative traders in making informed decisions based on the predicted stock trends. It's essential to keep in mind that the accuracy percentage should be interpreted carefully, as it might not fully represent the overall model performance due to the overfitting issue. You may need to further optimize the model, adjust hyperparameters, and explore additional techniques to improve its generalization and overall accuracy.
