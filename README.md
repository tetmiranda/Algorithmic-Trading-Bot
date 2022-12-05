# Background

![project-2-challenge](Images/proj2-background3.JPG)

# Project Goal
To investigate the potential feasibility of integrating different machine learning algorithms into conventional quantitative trading strategies with the aim of predicting buy and sell indicators within the cryptocurrency market space.  The cryptocurrency tokens selected for this anaylsis were Bitcoin, Ethereum, and Dogecoin.  

## About the project
The aim of this project was to create an algorithmic trading bot coupled with machine learning functionality with the primary goal of predicting buy and sell signals in order to generate profits in a hypothetical portfolio that surpasses a simple buy and hold stratagem. For this analysis, three crypto currencies were selected for their varying degrees of volatility, these were Bitcoin, Ethereum, and Dogecoin. The indicators tested were BB(Bollinger Band), EMA(Expontential Moving Averages), and RSI(Relative Strength Index) with entry and exit signals in order to predict the buy and sell signals. Lastly, our analysis compared four machine learning python modules to determine which machine learning would be better suited for algorithm trading. The machine learning modules that were tested are Logistic Regression, SVM, Random Forest Classifier, and Neural Networks (Keras).  

The strategy for this project was to pick the best trading strategy by virtue of profits generated during back testing and then test it against several machine learning packages to see which could best predict buy and sell indictors from the best trading strategy chosen. RSI was the clear winner for BTC and therefore was chosen to be tested against the chosen machine learning modules. This exercise was then repeated for ethereum and dogecoin, the results of which can be found in their respective notebooks.
  

 
## Data Preparation and Model Training
#### Data Preparation
 * Data sourced from Yfinance 
 * Period used to test - 2years with 1 hour intervals
 * Hourly returns were calculated and nulls dropped
 * Nulls dropped
 * Columns correctly renamed for later use
#### Signal Indicators
 * EMA crossovers
 * RSI
 * Bollinger Bands
### Machine Learning
#### Features
* RSI buy and sell signals
* Hourly BTC price
* Tading Volume
####  Logistic Regression Model
 * An algorithm that is used in solving classification problems. It is a predictive analysis that describes data and explains the relationship between variables.
####  SVM  
  *  Support vector machine is a model used for both classification and regression problems though it is mostly used to solve classification problems. 
#### Random Forest Classifier
 * Random Forest is a supervised learning algorithm used for both classification and regression problems.  Random forest builds multiple decision trees and merges them together to get a more accurate and stable prediction. This algorithm is common in various industries such as banking and e-commerce to predict behavior and outcomes.
#### Neural Network (Keras)
 * Keras is used by CERN, NASA, NIH, and many more scientific organizations around the world. Keras has the low-level flexibility to implement arbitrary research ideas.
#### Displaying Predicted Portfolio Outcomes
 * Using HVPlot
 
#### Summary of the analysis
 ### BITCOIN

**DATAFRAME**

<img width="790" alt="Screen Shot 2022-12-05 at 8 07 46 am" src="https://user-images.githubusercontent.com/108632632/205515686-5dec1fc3-9ed0-4dac-9585-b3bea2975c07.png">

* Screenshot of hourly BTC data before processing.

**EMA SIGNALS - ENTRY/EXIT**

<img width="978" alt="Screen Shot 2022-12-05 at 8 14 08 am" src="https://user-images.githubusercontent.com/108632632/205516032-e5bc73c2-c2bc-45d2-9d47-baaa17f250ef.png">

* EMA buy and sell signals graphed against 2 years of BTC close price data.

**EMA STRATEGY - TOTAL PORTFOLIO**

<img width="990" alt="Screen Shot 2022-12-05 at 8 15 49 am" src="https://user-images.githubusercontent.com/108632632/205516108-4f9ac047-83df-4893-a870-938f17238f11.png">

<img width="1092" alt="Screen Shot 2022-12-05 at 7 21 30 pm" src="https://user-images.githubusercontent.com/108632632/205588433-d3fe1054-adca-422e-8c94-3c44cdfc918e.png">

**RSI SIGNALS - ENTRY/EXIT**

<img width="988" alt="Screen Shot 2022-12-05 at 8 18 18 am" src="https://user-images.githubusercontent.com/108632632/205516214-575c75ec-cd61-4025-b8d3-b9e5a046ba02.png">

* RSI buy and sell signals graphed against 2 years of BTC close price data.


<img width="1004" alt="Screen Shot 2022-12-05 at 8 19 09 am" src="https://user-images.githubusercontent.com/108632632/205516259-30ab58e6-2822-49b7-a9bf-8c914838d5d1.png">

<img width="1085" alt="Screen Shot 2022-12-05 at 7 22 41 pm" src="https://user-images.githubusercontent.com/108632632/205588592-19a64691-c4f7-46bd-b5b3-dcb3e56149a1.png">

**BOLLINGER BANDS - ENTRY/EXIT**

<img width="996" alt="Screen Shot 2022-12-05 at 8 21 01 am" src="https://user-images.githubusercontent.com/108632632/205516340-38e3aaf1-b077-4e55-8026-202c92abc70e.png">

* Bollinger Band buy and sell signals graphed against 2 years of BTC close price data.

**BOLLINGER BANDS STRATEGY - TOTAL PORTFOLIO**

<img width="996" alt="Screen Shot 2022-12-05 at 8 21 43 am" src="https://user-images.githubusercontent.com/108632632/205516376-1cfc52da-d928-4c76-a258-2448d2e0184d.png">

<img width="1087" alt="Screen Shot 2022-12-05 at 7 24 55 pm" src="https://user-images.githubusercontent.com/108632632/205589156-2464e684-5339-4df4-9e88-58101fe728b7.png">

**SVM USING THE RSI STRATEGY**

![Screen Shot 2022-12-05 at 6 53 55 pm](https://user-images.githubusercontent.com/108632632/205586973-dcb7c820-9e79-4c68-ae58-adcdf9836c37.png)

* SVM results for predicting RSI buy(1) and sell(-1) signals.

<img width="554" alt="Screen Shot 2022-12-05 at 8 26 38 am" src="https://user-images.githubusercontent.com/108632632/205516573-3e26efd2-a9db-44b3-ab09-6aa0210759d8.png">

* Graph of buy and hold portfolio vs portfolio using SVM predicted signals.  

**LOGISTIC REGRESSION MODEL**

![Screen Shot 2022-12-05 at 6 54 48 pm](https://user-images.githubusercontent.com/108632632/205587528-d2f51c49-7711-414a-834f-46b8f6b13754.png)

* Logistic Regression results for predicting RSI buy(1) and sell(-1) signals.

<img width="673" alt="Screen Shot 2022-12-05 at 8 28 33 am" src="https://user-images.githubusercontent.com/108632632/205588022-91af9c32-4afa-4574-92ab-7b7a17072217.png">

* Graph of buy and hold portfolio vs portfolio using Logistic Regression predicted signals.  

**RANDOM FOREST CLASSIFIER**

![Screen Shot 2022-12-05 at 6 55 21 pm](https://user-images.githubusercontent.com/108632632/205587728-aeb53669-36df-408c-b381-f577c9e14b55.png)

* Random Forest Classifier results for predicting RSI buy(1) and sell(-1) signals.

<img width="554" alt="Screen Shot 2022-12-05 at 8 38 12 am" src="https://user-images.githubusercontent.com/108632632/205587936-da423ac4-9c27-473d-b695-a8d85ee4a656.png">

* Graph of buy and hold portfolio vs portfolio using Random Forest Classifier predicted signals.  

**NEURAL NETWORK**

<img width="560" alt="Screen Shot 2022-12-05 at 8 36 32 am" src="https://user-images.githubusercontent.com/108632632/205516956-16de8094-f718-408a-81a9-1e381f21ed00.png">

* Graph of buy and hold portfolio vs portfolio using Neural Network (Keras) predicted signals.  

This primary goal of this project was to validate the feasibility of integrating machine learning algorithms with standard quantitative trading strategies in the field of cryptocurrencies. As mentioned before, RSI was the prevailing strategy chosen for machine learning as it had the best outcome for BTC with a profit of 10.16% over two years. The machine learning results indicate that all machine learning modules and neural networks performed well at predicting RSI buy and sell signals using RSI, BTC price, and volume data as features. The SVM and Logistic Regression modules scored a recall (ratio of correct positive predictions to the total positives examples) metric above 75%, whereas, the Random Forest Classifier module displayed the best results all round scoring 99%. Likewise, the neural network performed admirably with an accuracy of 99%. However, despite these high degrees in accuracy scores for predicting buy and sells signals we saw all machine learning portfolio lose more money when compared to a buy and hold strategy. It is difficult to definitively explain why this is the case, however, there are several factors that are likely to have contributed to these lacklustre results.   

The first and mostly likely explanation is that the RSI signals were not well suited for the high degree of volatility seen in the cryptomarket. The RSI strategy did give the best result of 10.16% profit during the back testing phase of the experiment when compared to the other trading strategies. However, this level of profit does not permit a high degree of flexibility or repetition. Additionally, back testing results of different time lengths (1 year vs 2 years) showed less profit with the RSI strategy (data not shown). Secondly, the length of training given to the machine learning algorithms did not incorporate all the large swings in price data seen in recent months. Therefore, it could be suggested that the machine learning modules did well at learning when to buy and sell based of the feature set given, however, the feature set was inadequate for turning a profit in such a volatile market space.    

Based on these results incorporating a machine learning algorithm into a quantitative trading strategy could be beneficial, however, careful consideration must be given to the feature sets to be successful. Likewise, better preparation of data is also advised. Nevertheless, our findings suggest that the Random Forest Classifier was a clear front runner for this type of application among the machine learning modules chosen for this experiment. This is unsurprising as the Random Forest Classifier is often used in banking and market sectors due to being well suited for making predictions while able to mitigate the possibility of becoming overtrained to particular data sets.

## Challenges/Next steps

  * Finding an indicator that was well suited for crypto currencies
  * Time constraints to test different features
  * Testing different signals and values
  * Adding in costs per trade
  * Testing the Algorithmic Trading Bot on Stocks
  * Amending the code to better reflect the buy and sell signals

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
