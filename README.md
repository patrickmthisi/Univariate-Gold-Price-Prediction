# Univariate-Gold-Price-Prediction
## Project description and objectives:
The dataset consists of gold prices. For more information  about the data used in this project, refer to:

https://www.kaggle.com/datasets/sid321axn/gold-price-prediction-dataset.

In this end-to-end project, we develop a convolutional-long short-term memory (CNN-LSTM) model to provide daily forecasts of gold prices. The following essential concepts are explored in this project:
1. A univariate CNN-LSTM model is employed to forecast gold prices. An automated search of historical data is conducted to determine the optimal parameters, including filter and kernel sizes for the convolutions in the CNN layers, as well as the number of units for the LSTM component of the model.
2. Rolling Forecast: 
    - Once the model is fitted, a rolling forecast method is applied, allowing for predictions to be made one step ahead. The model is updated iteratively using actual values.
3. Model Evaluation:
    - The predicted values are compared to the actual values from the validation set.
    - The Root Mean Squared Error (RMSE) serves as the metric for assessing the model's performance.
    - Final predictions alongside the actual validation data are visualized.    
4. Conclusion and recommendation: The project also discusses potential future improvements, such as investigating other iterations of recurrent neural network models like the LSTM. Other predictive features can be incorporated to enhance prediction performance.

## Conclusion and recommendations
In this end-to-end project, we developed a univariate convolutional-long short-term memory (CNN-LSTM) model to forecast the daily price of gold. We used the persistence model as a baseline, which recorded an RMSE score of 0.30852. In contrast, our CNN-LSTM model outperformed this baseline, achieving an RMSE of 0.30775. An analysis of the residuals indicates that they follow a Gaussian distribution, although with fatter tails. Additionally, the autocorrelation plots show no evidence of serial correlation, suggesting that the CNN-LSTM model has successfully fitted the data. The model achieved the RMSE of 0.45128 using the out-of-sample validation dataset.

There are several potential avenues for improvement that could enhance performance. One approach is to incorporate predictive variables, which may lead to more accurate results. Additionally, exploring other artificial neural network (ANN) models, such as recurrent neural networks (RNN) and long short-term memory (LSTM) networks along with their variants, could also yield beneficial outcomes.
