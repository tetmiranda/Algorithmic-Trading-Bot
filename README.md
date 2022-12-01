# Background

![project-2-challenge](Images/proj2-background2.JPG)

# Project Goal
Create an algorithmic trading bot that successfully trades and outperforms the strategy of buying and holding.  The Crypto coins we have selected to use are Bitcoin, Ethereum and Dogecoin.  

## About the project
Our project is to create an algorithmic trading bot with machine learning that will generate profits at a speed and frequency that is not possible for human traders.  We have selected three crypto currencies to test our bot on (Bitcoin, Ethereum and Dogecoin). As the value of crypto is very volatile our aim is to offset some of this risk by introducing machine learning into our algorithim.  

Part of our analysis was to compare four machine learning modules to determine which machine learning would be better suited.  The machine learning modules we are using are Logistic Regression, SVM, Neural Networks (Keras) and Random Classifier.  

The indicators we used were BB(Bolinger Band), EMA(Expontential Moving Averages) and RSI(Relative Strength Index) with entry and exit signals in order to predict the total of the profit and loss.

 
## Data Preparation and Model Training
#### Data Preparation
 * Data sourced from Yfinance 
 * Period used - 2years with with 1 hour intervals
 * Hourly returns were calculated and nulls dropped
 * Nulls dropped
 * Columns correctly renamed for later use
#### Signal Indicators
 * Using EMA crossovers & overbought/oversold RSI and Bolinger Bands to predict when the right time to buy, sell and hold is.
#### Machine Learning
 * We will be using the Logistic Regression model to predict the future portfolio value based on the selected cryptocurrencies.
####  SVM Machine Learning
  * We incorporated the SVM Machine Learning into the Trading Strategy to predict/forecast the crypto price. We then backtested the testing predictions.
#### Neural Network (Keras)
 * Test neural networks and compare the predictions with the machine learning predictions.
#### Displaying Predicted Portfolio Outcomes
 * Using HVPlot
#### Summary of the analysis
 * BITCOIN


 * ETHERIUM



 * DOGE 
 
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
