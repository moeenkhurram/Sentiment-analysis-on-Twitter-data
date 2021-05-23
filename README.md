# Sentiment analysis on Twitter data

This repository contains the sentimental analysis on [Twitter data](https://www.kaggle.com/kazanova/sentiment140) downloaded from Kaggle. It contains 1,600,000 tweets extracted using the twitter api. Sentiment analysis is a type of NLP, and deals with the classification of emotions based on text data. The two main methods are : 
1. Rule-based sentiment analysis
2. Machine/Deep learning

Rule-based sentiment analysis 
======

It is one of the simplest approaches to determine text sentiments. It only requires minimal pre-work and the idea is quite simple, this method does not use any machine learning to figure out the text sentiment. The algorithm calculates the sentiment score from a set of manually created rules. For example, it can figure out the sentiments of a sentence by counting the number of times the user has used the word such as “great”,  “sad” in his/her tweet. 

Two popular methids were explored:
*  [TextBlob](https://textblob.readthedocs.io/en/dev/): Simplified Text Processing¶

Textblob sentiment analyzer returns two properties for a given input sentence: 

**Polarity** is a float that lies between [-1,1], -1 indicates negative sentiment and +1 indicates positive sentiments. 

**Subjectivity** is also a float which lies in the range of [0,1]. Subjective sentences generally refer to personal opinion, emotion, or judgment. 

*  [Valence aware dictionary for sentiment reasoning (VADER)](https://pypi.org/project/vaderSentiment/)

VADAR uses a list of lexical features (e.g. word) which are labeled as positive or negative according to their semantic orientation to calculate the text sentiment.   

Vader sentiment returns the probability of a given input sentence to be Positive, negative, and neutral. 

Machine/Deep learning 
======

In this method Bidirectional lstm model was build trained,  Long Short Term Memory networks (LSTM) are a subclass of RNN, specialized in remembering information for a long period of time. More over the Bidirectional lstms keep the contextual information in both directions.


References
------
+  https://towardsdatascience.com/lovecraft-with-natural-language-processing-part-1-rule-based-sentiment-analysis-5727e774e524
+  https://pypi.org/project/vaderSentiment/
+  https://textblob.readthedocs.io/en/dev/






