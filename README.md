# Background

![project-2-challenge](Images/proj2-background2.JPG)

# Project Goal
Create an algorithmic trading bot that successfully trades and outperforms the strategy of buying and holding.  The Crypto coins we have selected to use are Bitcoin, Ethereum and Dogecoin.  

## About the project
Our project is to create an algorithmic trading bot with machine learning that will generate profits at a speed and frequency that is not possible for human traders.  We have selected three crypto currencies to test our bot on (Bitcoin, Ethereum and Dogecoin). As the value of crypto is very volatile our aim is to offset some of this risk by introducing machine learning into our algorithim.  

Part of our analysis was to compare four machine learning modules to determine which machine learning would be better suited.  The machine learning modules we are using are Logic Regression, SVM, Neural Networks (Keras) and Random Classifier.  

The indicators we used were BB(Boolinger Band), EMA(Expontential Moving Averages) and RSI(Relative Strength Index) with entry and exit signals in order to predict the total of the profit and loss.

 
## Data Preparation and Model Training
#### Data Preparation
 * Data sourced from Yfinance
 * Nulls dropped
 * Columns correctly renamed for later use.
#### Signal Indicators
 * Using EMA crossovers & overbought/oversold RSI to predict when the right time to buy, sell and hold is.
#### Machine Learning
 * We will be using the Logistic Regression model to predict the future portfolio value based on the selected cryptocurrencies.
#### Neural Network (TensorFlow & Keras)
 * Test neural networks and compare the predictions with the machine learning predictions
#### Displaying Predicted Portfolio Outcomes
 * Using HVPlot
#### Concluding Analysis

 
## Technology
### Programming: Python 
### Libraries:
    * Skit-learn
    * Hvplot
    * Numpy
    * LogisticRegression model
    * Prophet 
    * Yfinance
