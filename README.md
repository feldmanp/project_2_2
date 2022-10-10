# Robo Advisor for Trading equities 

## Overview

### This robo advisor helps individuals with trading equities. Some features of this robo advisors are:


### - Interactions with the users 
### - Future stock prices forecast 
### - Provide technical analysis about the stock performance and the risks (Sharpe ratios & Sortino Ratio)  
### - Recommendations which includes trading strategies 

<br>

### An overview of the project: 
<p align="center">
  <img width="650" height="350" src="./Resources/mindmap.png">
</p>
---

<br>

## User instruction

<br>


### 1. Access AWS LEX bots 

### The user will navigate into this interface

<p align="center">
  <img width="300" height="550" src="Resources/lex1.png">
</p>

<br>

### 2. Input stock and holding period 

### User will tell the bot about their stock of interest and holding period:  

<p align="center">
  <img width="300" height="350" src="Resources/lex2.png">
</p>

**Note:** 
- The user must give **stock code** not the stock name. 
- The bot will produce price forecast for **a maximum of 3 months** worth of data. 

<br>

### 3. View results 

### The stock performance forecast: 
<p align="center">
  <img width="300" height="550" src="Resources/lex3.png">
</p>

### Using Moving average crossover trading algorithm: 
<p align="center">
  <img width="300" height="550" src="Resources/lex4.png">
</p>

### Sharpe Ratio: 

It gives insights about risk-adjusted performance of the stock. The mathematical expression is stock return rate minus risk free asset return rate, then divided by the total standard deviation of the stock return. 

For more information about Sharpe Ratio, visit: https://www.investopedia.com/terms/s/sharperatio.asp
<br>

### Sortino ratio: 

Sortino ratio also gives insights about the risk-adjusted performance of the stocks. While it is very similar with Sharpe Ratio, the difference is that Sortino Ratio uses the **downside standard deviation** rather than total standard deviation like Sharpe Ratio. 

**For more information about Sortino Ratio, visit: https://www.investopedia.com/terms/s/sortinoratio.asp. 

### Evaluating the model
<p align="center">
  <img width="650" height="350" src="">
</p>


***Precision-Recall Curve (not learnt in class):***

> 'The precision-recall curve shows the tradeoff between precision and recall for different threshold. A high area under the curve represents both high recall and high precision, where high precision relates to a low false positive rate, and high recall relates to a low false negative rate. High scores for both show that the classifier is returning accurate results (high precision), as well as returning a majority of all positive results (high recall).' - Scikit-learnt 

Source: https://scikit-learn.org/stable/auto_examples/model_selection/plot_precision_recall.html#:~:text=The%20precision%2Drecall%20curve%20shows,a%20low%20false%20negative%20rate.

<br>

## Installation guide: 

***Hvplot***

conda install -c pyviz hvplot

Source: https://hvplot.holoviz.org/getting_started/installation.html

<br>

***Scikit-learn***

pip install -U scikit-learn

Source: https://scikit-learn.org/stable/install.html

<br>


***Tensor Flow***

1. pip install --upgrade pip


2. pip install tensorflow


3. pip install tf-nightly

Source: https://www.tensorflow.org/install

<br>

***Yahoo Finance***

!pip install yfinance

Source: https://blog.quantinsti.com/historical-market-data-python-api/

***Prophet***


python -m pip install prophet
 

Source: https://facebook.github.io/prophet/docs/installation.html 


--- 
<br>

## Example: 
<br>

> ### ***Sam wants to invest in APPLE (stock code: AAPL) and he wants to hold the stock for 3 months. As an investor, Sam would like to get a good understanding about his investment idea. Sam would like to know th following:***
> <br>

> ### 1. What is the investment return after 3 months? 
> ### 2. How confident is robo advisor with the suggested return?  
> ### 3. How are the risks?  
> ### 4. Is there a way to improve the investment return results?
> <br>

> ###             ***The robo advisor can answer ALL!*** 

<br>

### Step 1: Input stock code and holding period to Robo Advisor. 

![]()

### Step 2: View 