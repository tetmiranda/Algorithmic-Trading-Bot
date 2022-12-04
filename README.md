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

<img width="778" alt="Screen Shot 2022-12-04 at 5 38 12 pm" src="https://user-images.githubusercontent.com/108632632/205478052-d62b315b-c83c-41ef-bbc2-84ea67f0bb1e.png">

TRADING SIGNAL USING RSI

<img width="492" alt="Screen Shot 2022-12-04 at 5 40 46 pm" src="https://user-images.githubusercontent.com/108632632/205478133-607c8354-392b-4679-a615-92962e2ec716.png">

GRAPH

<img width="997" alt="Screen Shot 2022-12-04 at 5 41 51 pm" src="https://user-images.githubusercontent.com/108632632/205478158-82adae31-3495-4867-a30a-a7d3f6bbbd75.png">

TOTAL PORTFOLIO VALUE

<img width="1003" alt="Screen Shot 2022-12-04 at 5 43 23 pm" src="https://user-images.githubusercontent.com/108632632/205478197-51f13c74-3e6e-4864-a43b-a7bbab8d002e.png">

Starting with a $100000.0 investment and using a 1 coin position size, the overall return of this algorithm is $10168.59 or 10.17%.
In comparison, buying and holding $100000.0 worth of BTC over the same time period would end up with a return of $-8313.34 or -8.31%.

SVM 

<img width="486" alt="Screen Shot 2022-12-04 at 5 53 16 pm" src="https://user-images.githubusercontent.com/108632632/205478461-ce115cb2-775b-44cd-ad53-269f2b3dfb9f.png">

<img width="384" alt="Screen Shot 2022-12-04 at 5 48 13 pm" src="https://user-images.githubusercontent.com/108632632/205478339-85291ba7-f9c2-4adf-89e9-0c830bb774e9.png">

LOGISTIC REGRESSION MODEL

<img width="476" alt="Screen Shot 2022-12-04 at 5 54 21 pm" src="https://user-images.githubusercontent.com/108632632/205478486-9802b802-154a-4d55-bae2-32479fe1675a.png">

<img width="381" alt="Screen Shot 2022-12-04 at 5 51 22 pm" src="https://user-images.githubusercontent.com/108632632/205478419-012c03ac-a5e5-4de3-9f49-c6c447c23aa1.png">

NEURAL NETWORK

<img width="381" alt="Screen Shot 2022-12-04 at 5 55 34 pm" src="https://user-images.githubusercontent.com/108632632/205478520-c45e50e7-4a91-475a-9768-e0062299523f.png">

RANDOM FOREST CLASSIFIER

<img width="447" alt="Screen Shot 2022-12-04 at 5 56 23 pm" src="https://user-images.githubusercontent.com/108632632/205478540-4d7e708b-3a45-4dcc-ada3-560592cc20ed.png">

<img width="380" alt="Screen Shot 2022-12-04 at 5 56 31 pm" src="https://user-images.githubusercontent.com/108632632/205478547-180f3996-8b69-490c-b5f1-dd2948fa48ec.png">

We ran the above analysis for Etherium and Doge please feel free to review the notebooks specific to these codes.

The returns don't perform and we don't recommeding using the machine learning model with these indications.

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
   
## Bot Team Members
   *  Rita Thomas
   *  Dennis Mader
   *  Lachlan Andrews
   *  David Newman
   *  Florante Miranda 
