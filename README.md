# Twitter Sentiment Analysis
Text Processing and Sentiment Analysis of Twitter Data.


### Abstract
Sentiment Analysis is the most common text classification tool that analyses an incoming message and tells us the underlying sentiment. Twitter contains huge data about users and the relationships between them. The linguistic analysis of Twitter has been applied as a tool to understand the behavior between individuals or organizations.  The main purpose of this work has been to carry out text processing and sentiment analysis of Twitter data. The Twitter sentiment analysis has been applied over five different American airlines and their corresponding polarity (positive or negative). Three supervised classifiers have been used: Random Forest, Logistic Regression and SVM. The results show that the classifier that has provided the best results has been SVM: 0.84 of both accuracy, precision, recall and F1. However, the results do not vary considerably if we compare them with those obtained with the Logistic Regression classifier: 0.83 accuracy, 0.83 precision, 0.84 recall and 0.83 F1.


### Project Files
-	Requirements.txt : file where all the necessary libraries are to carry out the execution of the model and the exploratory of the data. It is highly encouraged to run the project on a new python environment. Afterwards, activate the new environment created and install the necessary libraries running the following instruction in your console: pip3 install -r requirements.txt

-	Data (Tweets.csv): the dataset with the necessary data to make the classification model.

-	TfM_Explo_Desc_V1: An exploratory analysis of the data is carried out (tweets.csv), each of the fields that make up the dataset are explored and those that are considered useful for the project are selected. In addition, the fields selected as useful are also related to each other and the results are represented by graphs. Finally, the Wordcloud library is used for representing text in which the size of each word indicates its frequency or importance.

-	TfM_Sentiment_Analysis_V2: The data is imported, a dataframe is created with the columns that were considered useful for the project and the data is cleaned. To begin with, those 'neutral' labels that belong to the 'airline_sentiment' field are replaced by the 'positive' name, so that the set of labels is only positive / negative. Next, the preprocessing of the text is carried out. However, for each of the previous steps it is verified that the extracted results are the correct ones. Regarding the preprocessing of the text of the tweets, the main procedures have been the following: 
		- Elimination of hastags, mentions and link
		- Elimination of emojis
		- Treatment of linguistic contractions
		- Treatment of emoticons
		- Treatment of punctuation marks, uppercase characters, etc.	
		- Lemmatization

-	TfM_Sentiment_Analysis_Classifiers_V3: Mainly the preprocessing of each of the tweets is done again and some graphs are made to provide clearer and more precise information about the type of data with which we are going to work. Next, a Bag of Words is created with the 6000 most frequent tokens without stopwords and CountVectorizer is used to convert to collection of text documents to a matrix of token counts. Then, with this obtained data, a TF-IDF model is created to transform a count matrix (X) to a normalized tf-idf representation (X). Tf means term-frequency while tf-idf means term-frequency times inverse document-frequency. Subsequently, the data obtained from the TF-IDF model, as well as their respective labels with the respective sentiment of each of the tweets, are divided into a training set and a test set. Finally, each of the classifiers is applied and results of its correct operation are extracted through a series of graphs of their respective matrices of confusion.

-	TfM_Sentiment_Analysis_Opt_Classifiers_V4: This is the last notebook created for the creation of the classification model. The main objective of this notebook is to optimize the results obtained so far and provided in the TfM_Sentiment_Analysis_Classifiers_V3 notebook. The main difference between this notebook and the previous notebook is that it uses the Tfidfvectorizer model and the previous one uses Tfidftransformer. The differences between the two modules can be quite confusing: with Tfidftransformer we will systematically compute the word counts with CountVectorizer, generate Inverse Document Frequency (IDF) values and then compute Tf-idf scores. However with Tfidfvectorizer we will do all three steps at once. Under the hood, it computes the word counts, IDF values, and Tf-idf scores all using the same dataset.	

-	Tableau: The graphics made with the Tableau tool, where the data is displayed.

-	TFM: the entire project written and explained.


### Tableau
This section shows us the links to view through dashboards, how sentiment analysis has been applied over 5 different American airlines and their corresponding polarity. The links are the following:

Tweets Airline Sentiment vs. Airline
https://public.tableau.com/profile/raul3410#!/vizhome/Num_AirlineSentimentVs_Airline/Num_AirlineSentimentvs_Airline?publish=yes

Negative Analysis
https://public.tableau.com/profile/raul3410#!/vizhome/NegativeTweetAnalysis/Dashboard1?publish=yes

Records and Reasons by Sentiment
https://public.tableau.com/profile/raul3410#!/vizhome/Records_Reasons_by_Sentiment/RecordsandReasonsbySentiment?publish=yes

Number of  Retweets ~ Airline Sentiment by Airline
https://public.tableau.com/profile/raul3410#!/vizhome/TweetsvsRetweets2/Num_ofRetweets_AirlineSentimentbyAirline?publish=yes

Tweets vs Retweets ~ Airline Sentiment by Airline
https://public.tableau.com/profile/raul3410#!/vizhome/TweetsvsRetweets3/TweetsvsRetweets?publish=yes

