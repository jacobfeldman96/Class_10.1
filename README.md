# Class 10.1

### November 14, 2020

Today's topics included Time Series Analysis and Machine Learning. Today's class began with the buzzword concepts of machine learning and artificial intelligence.

Narrow artificial intelligence, as opposed to general artificial intelliege (a moral, thinking robot), is technological and exists physically. The components of narrow AI are Machine Learning, Reinforcement Learning, Deep Learning and Natural Language Processing. 

What is machine learning? Machine learning is a component of Narrow AI that is comprised of statistical techniques and algorithms that allows one to work with big, labeled, or unlabeled data. One programs such a dataset with an algorithm and allows the algorithm to learn, adjust and predict future outcomes without manual configuration. Machine learning is currently being deployed in most sectors of the economy, including: markets and finance, medicine, consumer segmentation, governmental elections and natural disaster, planetary and climate geological impacts.

Many machine learning algorithms are available in the open sourced community. The three major components of machine learning are model -> fit -> predict. Intelligent algorithms learn by themselves and evolve into better algorithms.

There are two types of Machine Learning: supervised and unsupervised learning.  Supervised learning uses labeled data for classification models such as: image classification, indentity, customer retention, diagnostics, and regression models: linear regression, population growth, advertising's popularity prediction, weather forecasting, market forecasting and life expectancy.  Unsupervised learning uses unlabeled data and tries to recognize emerging patterns into meaningful compressed data. Used for big data visualization, structure discovery, and future elicitation. It further clusters data for system recommendation, targeted marketing and customer segmentation. 

Reinforcement learning is used for real-time decision making, robot navigation, game AI and skill acquisition. 

These algorithms all fall under the broader and general business term of predictive analytics. 

The three main providers for machine learning infrastructure are Microsoft's Azure, Google's Tensorflow and Amazon Web Services. 
___

This week we will be focusing on time series (TS) and linear regression. 

 Topics today included: stationary vs non-stationary data sets, decomposition, multiplicity, EWMA and Hodrick-Prescott Equations. 

A stationary data set is a TS that has had an equation performed on it. For example .pct_chang() transforms a TS of closing prices into a stationary data set. 

Decomposition - why do we need it? Because breaking down a TS into the four components allows a better understanding of the actual time series. The four components of a time series are: level (avg value), trend (overall pattern), periodicity/cycle (when) and residual/error/noise (the immediate volatility within a trend line).The two most useful are trend and perodicity and the two least useful are noise and level. 

Upward trend + preodicity = multiplicity 

Simplest way to decompose a TS is via the statsmodels.tsa.seasonal library and importing seasonal_decompose. 

EWMA = Exponentially Weighted Moving Average. Why and when would we use ewma? To smooth out trend lines for non-cash cow companies, when recent data is more relevant for analysis. 

What is Hodrick-Prescott Equation? An equation that minimises noise and volatility and bolsters the long term trend effect. 

Lastly, when reviewing data if the trend and noise lines have a similar trajectory in their plots, one can see a major economic event. 