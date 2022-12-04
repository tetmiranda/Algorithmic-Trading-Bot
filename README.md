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
 * BITCOIN


 * ETHERIUM



 * DOGE 
 
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
   
## Bot Team Members
   *  Rita Thomas
   *  Dennis Mader
   *  Lachlan Andrews
   *  David Newman
   *  Florante Miranda 
