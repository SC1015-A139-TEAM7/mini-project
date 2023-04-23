# SC1015 Mini Project

## About

This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which has the objective of finding the best methodology to predict stock price. 

We used the S&P 500 stock data taken from [Alphavantage API](https://www.alphavantage.co/). Data extraction and preprocessing is in this file: link the [data preprocessing notebook](src/data-preprocessing.ipynb)

You can find the video explanation of our mini project [here](https://youtu.be/dn-l954J71o)

## Contributors
- @joankadevi - Data Visualisation, Data Analysis, MA, LSTM, Slides and Video editing
- @JeremyNathanJusuf - Data Extraction, NAIVE, MA, Exponential Smoothing, LSTM, Data Analysis

## Problem Definition
In today's fast-paced world, the stock market is one of the most popular avenues for investments. However, predicting stock prices accurately is a challenging task that requires advanced techniques and tools as the stock market is complex and volatile. 

Investors are looking for an accurate and reliable predictive model which can capture the market’s highly volatile and nonlinear behavior. 

That's where our project comes in. Our objective is to find the best forecaster to predict stock prices using various techniques and a machine learning model. By doing so, we hope to help individual investors make better-informed decisions about their investments.

## Statistical and Machine Learning Models 
1. [NAIVE METHOD](src/naive-method.ipynb)
2. [MOVING AVERAGE](src/moving-average.ipynb)
3. [EXPONENTIAL SMOOTHING](src/exponential-smoothing.ipynb)
4. [LONG SHORT-TERM MEMORY NETWORKS](src/LSTM-model.ipynb)


## Conclusion

We used RMSE as the model performance metric for our experiment.
RMSE values obtained by our models (in USD):

1. NAIVE METHOD: 4.617 
2. MOVING AVERAGE WINDOW SIZE 5: 6.472 
3. EXPONENTIAL SMOOTHING WITHOUT TREND: 4.599 
4. EXPONENTIAL SMOOTHING WITH TREND: 4.631 
5. LSTM: 7.299 

Hence, we can conclude that the best method to predict future stock price is exponential smoothing without trend as it has the lowest RMSE value indicating that it is the most accurate method. However, this such RMSE is still considered large in the context of predicting stock prices and would need further improvements to produce more accurate predictions.

## Further Improvements
The LSTM model is a very promising model to predict stock price as well. In this case we can actually improve our model of LSTM by implementing other learnable indicators for the model to study from, for example the relative strength index, USD index, news, consumer sentiment index, unemployment rate, etc. Besides, we can tune better hyper parameters for the LSTM model to be more accurate.

## What we learnt from this project
- Theory of stock movements
- Collecting data through API request
- Recurrent Neural Networks (Particularly LSTM), Keras, Tensorflow
- Mathematical conceptsof NAIVE, Moving Average, Exponential Smoothing and LSTM
- Hyperparameters of models mentioned and how to find the most optimal one
- Implementation of the statistical and ML models mentioned in Python
- Project collaboration using GitHub

## References
- Author links open overlay panelHum Nath Bhandari a, a, b, c, d, e, f, &amp; AbstractThe rapid advancement in artificial intelligence and machine learning techniques. (2022, May 13). Predicting stock market index using LSTM. Machine Learning with Applications. Retrieved April 22, 2023, from https://www.sciencedirect.com/science/article/pii/S2666827022000378
- YouTube. (2020, November 27). Predicting stock prices with lstms: One mistake everyone makes (episode 16). YouTube. Retrieved April 22, 2023, from https://www.youtube.com/watch?v=Vfx1L2jh2Ng
- Alpha Vantage API Documentation. API Documentation | Alpha Vantage. (n.d.). Retrieved April 22, 2023, from https://www.alphavantage.co/documentation/
