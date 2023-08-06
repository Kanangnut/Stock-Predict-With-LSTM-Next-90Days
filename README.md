<b>Stock Price Prediction of Tesla Inc Stock for Next 90 days using Long Short-Term Memory (LSTM)</b><br>
This project using LSTM Recurrent Neural Network for prediction of TSLA stock.

<b>Dataset:</b><br>
The dataset is taken from yahoo website in CSV format.The dataset consists of Open, High, Low, Close, Adj Close Prices and Valume of Tesla Inc. stocks from 29th Jun 2010 to 19th July 2023.<br>

<b>Indicator:</b><br>
Stock traders mainly use OHLC average for prediction.<br>

<b>Processing and Model</b><br>
After converting dataset into OHLC average, this has been convert into column of time series data. Then transform to training and test data in the form of previous days. And  input on LSTM model. Following 2 stacked LSTM layers with 1 dense layer, 2 sequences then calculate training and testing Root Mean Square Error (RMSE).

<b>Version<b><br>
Python 3.11.2 and deep learning library Keras and Tensorflow.<br>

The trining and testing of OHLC average price:
![image](https://github.com/Kanangnut/Stock-predict-with-LSTM-for-next-3-month/assets/130201193/f5b956fc-77d8-4494-9995-6145d6ee8aec)

Finally, we plot the Original OHCL dataset with Forecast OHCL values, orange line show forecast values of the next 3 month.<br>
![image](https://github.com/Kanangnut/stock-predict-with-LSTM-for-next-3-month/assets/130201193/b298300c-01e7-4a9c-9144-a528fa3e8335)

<b>Observation:</b><br>
Since difference among of the training and testing RMSE are 0.68 and 8.63 respectively, from the testing result quit higher than the training set. It likely this model badly over fit of the data. However stock price from the last day of data set was 294.0275 and using this model abd price of next three days are predicted as 307.7730, 261.8300 and 265.2500 - which were 271.1475, 262.955 and 262.2200 on 20th, 21th and 24th July 2023 according to yFinance. From the result accuracy show at 95.79%, so the trend of future values of any time period can be predicted usind this model. In my view, this work can help the quantitative traders to take decisions.

<b>Conclusion:</b><br>
The model's overfitting to the training data is a concern, and it may not perform well on unseen data. However, the predictions are reasonably accurate, suggesting that the model can help predict the trend of future stock prices with a relatively high level of confidence. The model's performance could be beneficial for quantitative traders in making informed decisions based on the predicted stock trends. It's essential to keep in mind that the accuracy percentage should be interpreted carefully, as it might not fully represent the overall model performance due to the overfitting issue. You may need to further optimize the model, adjust hyperparameters, and explore additional techniques to improve its generalization and overall accuracy. Additionally, always consider using a separate validation set or cross-validation to get a more robust estimate of the model's performance on unseen data.
