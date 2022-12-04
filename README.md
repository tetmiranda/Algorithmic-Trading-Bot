# Background

![project-2-challenge](Images/proj2-background3.JPG)

# Project Goal
Create an algorithmic trading bot that successfully trades and outperforms the strategy of buying and holding.  The Crypto coins we have selected to use are Bitcoin, Ethereum and Dogecoin.  

## About the project
Our project is to create an algorithmic trading bot with machine learning that will generate profits at a speed and frequency that is not possible for human traders.  We have selected three crypto currencies to test our bot on (Bitcoin, Ethereum and Dogecoin). As the value of crypto is very volatile our aim is to offset some of this risk by introducing machine learning into our algorithim.  

Part of our analysis was to compare four machine learning modules to determine which machine learning would be better suited.  The machine learning modules we are using are Logistic Regression, SVM, Neural Networks (Keras) and Random Forest Classifier.  

The indicators we tested were BB(Bollinger Band), EMA(Expontential Moving Averages) and RSI(Relative Strength Index) with entry and exit signals in order to predict the buy and sell signals.  Many of these indicators failed.  We used the RSI in our final trading strategy.  

 
## Data Preparation and Model Training
#### Data Preparation
 * Data sourced from Yfinance 
 * Period used to test - 2years with 1 hour intervals
 * Hourly returns were calculated and nulls dropped
 * Nulls dropped
 * Columns correctly renamed for later use
#### Signal Indicators
 * Using EMA crossovers & overbought/oversold RSI and Bollinger Bands to predict when the right time to buy, sell and hold is.
### Machine Learning
####  Logistic Regression Model
 * We will be using the Logistic Regression model to predict the future portfolio value based on the selected cryptocurrencies.
####  SVM  
  * We incorporated the SVM Machine Learning into the Trading Strategy to predict/forecast the crypto price. We then backtested the testing predictions.
#### Neural Network (Keras)
 * Test neural networks and compare the predictions with the machine learning predictions.
#### Random Forest Classifier
 * Random Forest is a supervised learning algorithm used for both classification and regression problems.  Random forest builds multiple decision trees and merges them together to get a more accurate and stable prediction.

#### Displaying Predicted Portfolio Outcomes
 * Using HVPlot
 
#### Summary of the analysis
 ### BITCOIN

DATAFRAME

<img width="790" alt="Screen Shot 2022-12-05 at 8 07 46 am" src="https://user-images.githubusercontent.com/108632632/205515686-5dec1fc3-9ed0-4dac-9585-b3bea2975c07.png">

EMA SIGNALS - ENTRY/EXIT

<img width="978" alt="Screen Shot 2022-12-05 at 8 14 08 am" src="https://user-images.githubusercontent.com/108632632/205516032-e5bc73c2-c2bc-45d2-9d47-baaa17f250ef.png">

EMA STRATEGY - TOTAL PORTFOLIO

<img width="990" alt="Screen Shot 2022-12-05 at 8 15 49 am" src="https://user-images.githubusercontent.com/108632632/205516108-4f9ac047-83df-4893-a870-938f17238f11.png">

Starting with a $100000.0 investment and using a 1 coin position size, the overall return of this algorithm is $5972.44 or 5.97%.
In comparison, buying and holding $100000.0 worth of BTC over the same time period would end up with a return of $-8579.23 or -8.58%.

RSI SIGNALS - ENTRY/EXIT

<img width="988" alt="Screen Shot 2022-12-05 at 8 18 18 am" src="https://user-images.githubusercontent.com/108632632/205516214-575c75ec-cd61-4025-b8d3-b9e5a046ba02.png">

This is the buy/sell chart.  Red indicates sell and Green indicates buy.

RSI STRATEGY - TOTAL PORTFOLIO

<img width="1004" alt="Screen Shot 2022-12-05 at 8 19 09 am" src="https://user-images.githubusercontent.com/108632632/205516259-30ab58e6-2822-49b7-a9bf-8c914838d5d1.png">

Starting with a $100000.0 investment and using a 1 coin position size, the overall return of this algorithm is $10417.29 or 110.42%.
In comparison, buying and holding $100000.0 worth of BTC over the same time period would end up with a return of $-8579.23 or -8.58%.

BOLLINGER BANDS - ENTRY/EXIT

<img width="996" alt="Screen Shot 2022-12-05 at 8 21 01 am" src="https://user-images.githubusercontent.com/108632632/205516340-38e3aaf1-b077-4e55-8026-202c92abc70e.png">

This is the buy/sell chart.  Red indicates sell and Green indicates buy.

BOLLINGER BANDS STRATEGY - TOTAL PORTFOLIO

<img width="996" alt="Screen Shot 2022-12-05 at 8 21 43 am" src="https://user-images.githubusercontent.com/108632632/205516376-1cfc52da-d928-4c76-a258-2448d2e0184d.png">

Starting with a $100000.0 investment and using a 1 coin position size, the overall return of this algorithm is $-16313.15 or 83.69%.
In comparison, buying and holding $100000.0 worth of BTC over the same time period would end up with a return of $-8579.23 or -8.58%.

SVM USING THE RSI STRATEGY

<img width="634" alt="Screen Shot 2022-12-05 at 8 33 30 am" src="https://user-images.githubusercontent.com/108632632/205516831-25436893-4968-49a3-b230-9819b105b9a3.png">


<img width="554" alt="Screen Shot 2022-12-05 at 8 26 38 am" src="https://user-images.githubusercontent.com/108632632/205516573-3e26efd2-a9db-44b3-ab09-6aa0210759d8.png">

LOGISTIC REGRESSION MODEL

<img width="582" alt="Screen Shot 2022-12-05 at 8 34 16 am" src="https://user-images.githubusercontent.com/108632632/205516852-84d49d95-d42b-425b-9449-8db133a22a0b.png">

<img width="673" alt="Screen Shot 2022-12-05 at 8 28 33 am" src="https://user-images.githubusercontent.com/108632632/205516684-93df2df9-05a0-46d8-a74d-75ee5ec22bc8.png">

NEURAL NETWORK

<img width="560" alt="Screen Shot 2022-12-05 at 8 36 32 am" src="https://user-images.githubusercontent.com/108632632/205516956-16de8094-f718-408a-81a9-1e381f21ed00.png">


RANDOM FOREST CLASSIFIER

<img width="635" alt="Screen Shot 2022-12-05 at 8 35 16 am" src="https://user-images.githubusercontent.com/108632632/205516893-9d9c1001-1902-4357-bfe9-c39b3aa2c2d2.png">

<img width="554" alt="Screen Shot 2022-12-05 at 8 38 12 am" src="https://user-images.githubusercontent.com/108632632/205517003-7d4a890a-08f8-4899-b3e3-449d8ec0399a.png">


We ran the above analysis for Etherium and Doge please feel free to review the notebooks specific to these codes.

The returns don't perform and we don't recommeding using the machine learning model with these indicators.

In summary, xxxxxx 
 

 
The precision (ratio of correct positive predictions to the total predicted positives) between the logistic regression and svm model is relatively similar with the exception of the svm training report, which shows a slight dip in the sell signals (-1). However, the logistic regression model shows a much higher yet still relatively weak recall (ratio of correct positive predictions to the total positives examples) when compared to the svm models. Furthermore, the logistic regression model has a higher accuracy when compared with the svc model.
 
Interestingly, the predicted trading algorithm returns fairs better in the svm model compared to the regression model when plotted out. Though, based on this machine learning model reports, these graphs should be taken with a grain of salt.

It is difficult to compare the neural network outcome with the machine learning reports due to different measures of accuracy. Nevertheless, the high degree of accuracy coupled with the neural network algorithm returns plot suggests that it is not a wise investment stratergy.
 
## Technology
#### Programming: Python 
#### Libraries:
   * Pandas - Pandas is a Python library used for working with data sets. It has functions for analyzing, 
     cleaning, exploring, and manipulating data.
   * Yfinance - open source library to access the financial data available on Yahoo Finance. 
   * Scikit-learn - is a free machine learining library for Python.  It features various algorithms like support vector machine, 
     random forests, and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy .
   * Hvplot - provides an alternative for the static plotting API provided by Pandas and other libraries, with by default 
     an interactive Bokeh-based plotting API that supports panning, zooming, hovering, and clickable/selectable legends.
   * Numpy - is a library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, 
     along with a large collection of high-level mathematical functions to operate on these arrays.
   * Finta - offers common financial technical indicator implemented in Pandas.
   * Matplotib - is a cross-platform, data visualization and graphical plotting library for Python and its numerical extension NumPy.
   * TensorFlow - is an open-sourced end-to-end platform, a library for multiple machine learning tasks, while Keras is a high-level neural network          library that runs on top of TensorFlow.  Keras is an open-source software library that provides a Python interface for artificial neural                networks. Keras acts as an interface for the TensorFlow library.
   
## Bot Team Members
   *  Rita Thomas
   *  Dennis Mader
   *  Lachlan Andrews
   *  David Newman
   *  Florante Miranda 
