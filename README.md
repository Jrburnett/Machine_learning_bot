# Machine_learning_bot
machine learning trading bot
# Libraries 
- import pandas as pd
- import numpy as np
- from pathlib import Path
- import hvplot.pandas
- import matplotlib.pyplot as plt
- from sklearn import svm
- from sklearn.preprocessing import StandardScaler
- from pandas.tseries.offsets import DateOffset
- from sklearn.metrics import classification_report
# Purpose
## Establish Baseline Performance
In establishing a baseline performance I imported the data that I needed, cleaned said data, and added SMA slow and fast, followed by a signal column that tells when to buy or sell. I then created strategy returns by mulitplying actual returns by the prior trading singal. I then implemented the first machine learning ascpect by setting up my svm model. 
## Tune the Baseline Trading Algo
### Step 1: Tune the training algorithm by adjusting the size of the training dataset. 
- Answer the following question: What impact resulted from increasing or decreasing the training window?
- The less amount of data in the training window the less the machine learning model can learn from and the less accurate the model will be.
### Step 2: Tune the trading algorithm by adjusting the SMA input features. 
- Answer the following question: What impact resulted from increasing or decreasing either or both of the  SMA windows?
- The impact from increasing and or decreasing the sma windows can be seen in the PNG files.
## Evaluate a New Machine Learning Classifier
The second machine learning model I used was the decision tree model, this model performed similar to the previous model, towards the end but throughout performed different. You can see the results of this module in the decision_tree_Model.PNG.
# Conclusion
All of the models tested can be seen in the PNG files below. In order to get a better machine learning bot, I would advise in adding more technical indicators and creating better signals that you can feed into your machine learning bot.

![image](https://github.com/Jrburnett/Machine_learning_bot/blob/main/Images/decision_tree_Model.PNG)

![image](https://github.com/Jrburnett/Machine_learning_bot/blob/main/Images/svm_Model.PNG)

![image](https://github.com/Jrburnett/Machine_learning_bot/blob/main/Images/svm_Model_50MA.PNG)

![image](https://github.com/Jrburnett/Machine_learning_bot/blob/main/Images/svm_Model_150MA.PNG)

![image](https://github.com/Jrburnett/Machine_learning_bot/blob/main/Images/svm_Model_200MA.PNG)