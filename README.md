# COVID19-Urban-Sentiment-Analysis

This is a data analysis study on the period one week before and after the COVID-19 quarantine was put in Egypt, This analysis investigates social media activity and sentiment for each Egyptian governorate in terms of its urban features and its activity regarding the COVID-19 pandemic.

The study proposes four different approaches for text data mining for spatio-temporal labelled data on Twitter and apply various NLP techniques for preprocessing before building a machine learning based model for sentiment classification and a dictionary for COVID-19 tweets detection.

## Sample of the results
Sentiment of the people during the weeks before and after quarantine measures were imposed on the 14th of March halting all education on campus.

![Sentiment Analysis](/Graphs/SentimentDateAll.png)

Pie chart of the percentage of COVID-19 tweets from all extracted tweets and a Word cloud extracted for the most mentioned words regarding COVID-19

![Corona Pie](/Graphs/PieChartCoronaMentions.png) ![Word Cloud](/Graphs/CoronaWordCloud.png)

## Creating the Egyptian Governorates dataset
I collected info on Egyptian governorates needed for the data collection and results in the future. I collected from three different sources the features needed using Pandas read-html for tables and combined them into one single dataset.

## Twitter Data Mining
The study uses the TWINT tool in https://github.com/twintproject/twint to scrap tweets from Twitter overcoming the tweets limit of the Twitter API and session time
I propose four different appraoches to extract spatially unlabelled tweets with respect to a certain area or city
* Geotagged Approach
* Keyword Search Approach
* Profile Info Approach
* Nearby Location Approach

## Preprocessing and Sentiment Analysis
I have used the Arabic sentimentally annotated dataset from https://github.com/iamaziz/ar-embeddings and an English annotated dataset for building our model both found in our datasets folder.

For NLP I have used regex techniques to normalize the tweet from unnecessary formats, emojis, numbers and punctuations and used the Tashaphyne Arabic light stemmer from https://pypi.org/project/Tashaphyne/ to lightly stem the tweed used NLTK corpus on stopwords to remove Arabic stopwords.

To build the model, I used Scikit-learn's Count Vectorizer on unigrams and bigrams collection and TF-IDF transformer to extract text features from tweets into a TF-IDF matrix and a Naive Bayes classifier through a pipeline to build our model over the stemmed tweets.

## COVID-19 Detection in Tweets
I have made a dictionary of the most common terms related to the coronavirus and used them to detect the tweets containing them to declare it a COVID-19 tweet.
