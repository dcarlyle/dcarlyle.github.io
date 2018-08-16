---
title: "LSTM time sequence analysis"
header:
  overlay_image: /assets/images/data.jpeg
  caption: "Photo credit: [Markus Spiske](https://unsplash.com/@markusspiske)"
  cta_url: "https://github.com/dcarlyle/stocks_ml/blob/master/stockdemo.ipynb"
categories:
  - Machine learning
  - FinTech
tags:
  - Machine Learning
  - FinTech
last_modified_at: 2017-08-18T11:45:09-04:00
---

# Stock prediction
Quantitative analysis of *certain variables* and their correlation with stock price behaviour. This used to be hard, but now with powerful tools and libraries like tensorflow it is much simpler.

In the 1980's two British statisticians, Box and Jenkins, created a mainframe program to attempt to predict stock prices from just two data points, price and volume. It was known as Autoregressive Integrated Moving Average (ARIMA).

The Box-Jenkins approach claims that non-stationary data can be made stationary by differencing the series, Y<sub>t</sub> :

Y<sub>t</sub> = &Phi;<sub>1</sub>Y<sub>t-1</sub>+&Phi;<sub>2</sub>Y<sub>t-2</sub>...&Phi;<sub>&rho;</sub>Y<sub>t-&rho;</sub>+&epsilon;<sub>t</sub>+&theta;<sub>1</sub>&epsilon;<sub>t-1</sub>+&theta;<sub>2</sub>&epsilon;<sub>t-2</sub>+...&theta;<sub>q</sub>&epsilon;<sub>t-q</sub>

The ARIMA model combines three basic methods:

1. *AutoRegression (AR)* – Auto-regression, the values of a given time series data are regressed on their own lagged values, which is indicated by the “p” value in the model.
2. *Differencing (I-for Integrated)* – Conversion of a non-stationary time series to a stationary one to remove time trends. This is indicated by the “d” value in the model. If d = 1, it looks at the difference between two time series entries, if d = 2 it looks at the differences of the differences obtained at d =1, and so forth.
3. *Moving Average (MA)* – The moving average nature of the model is represented by the “q” value which is the number of lagged values of the error term.


## A modern approach using artificial intelligence (AI)
The code below uses Keras, an API used to simplify prototyping on top of AI frameworks like Google's Tensorflow. Google Tensorflow has its own flavour of Keras, which I use below with Python 3.6 to build a deep learning model.

The very simple approach below uses only a single data point, the *closing price* with a deep neural network of only 2 layers using time sequence analysis recurrent networks variant LSTMs.

### Data set
Our data is from the daily closing prices from S&P 500 from Jan 2000 to Aug 2016. The series is index in time order.

### Goal
Our goal is to predict the closing price for any given date.






