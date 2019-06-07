# Twitter Sentiment Analysis
Text Processing and Sentiment Analysis of Twitter Data.


### Abstract
Sentiment Analysis is the most common text classification tool that analyses an incoming message and tells us the underlying sentiment. Twitter contains huge data about users and the relationships between them. The linguistic analysis of Twitter has been applied as a tool to understand the behavior between individuals or organizations.  The main purpose of this work has been to carry out text processing and sentiment analysis of Twitter data. The Twitter sentiment analysis has been applied over five different American airlines and their corresponding polarity (positive or negative). Three supervised classifiers have been used: Random Forest, Logistic Regression and SVM. The results show that the classifier that has provided the best results has been SVM: 0.84 of both accuracy, precision, recall and F1. However, the results do not vary considerably if we compare them with those obtained with the Logistic Regression classifier: 0.83 accuracy, 0.83 precision, 0.84 recall and 0.83 F1.



### Requeriments:
It is highly encouraged to run the project on a new python environment:

conda create -n ptfenv python=3.7.1

Afterwards, activate the new environment created (named 'Twitter_Data') and install the necessary libraries running the following instruction in your console:

pip3 install -r requirements.txt
