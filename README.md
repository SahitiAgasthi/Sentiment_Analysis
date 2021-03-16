# Sentiment_Analysis
A sentiment analysis job about the problems of each major U.S. airline.
The dataset consists of Tweets and corresponding sentiment negative, neutral, or positive. The tweets are in the text column of the data and sentiment is in the Target column. The Target column has three values: 1,-1, 0 that corresponds to positive, negative, and neutral sentiment respectively. My task will be to train the model to predict the sentiment of the tweets.

The evaluation metric for this competition is Macro F-Score.

Approach taken:
1. To pre-process the tweets, I have used Tokenization, Stopword removal and Stemming (Porter Stemmer).
2. To convert tokens to text, count vectorization (bag of words) approach has been used.
3. Machine Learning model used for this classification is Logistic Regression. The best Macro score obtained using this model is 0.7192.
4. Predicted the outcome of Tweets(text) and stored them under result.csv file.

# The data description
The data set three files: train.csv, test.csv.
The train.csv has three columns: id, text, and Target. text column has Tweets and Target column has sentiments (-1,0,1). In the Target column, values of -1,1,0 correspond to negative, positive, and neutral sentiment.

I have to train my model using the train.csv file and make predictions on the test.csv file. I cannot use test.csv in training my model as it does not have labels (outcome). My task is to predict the outcome for Tweets(text) in test.csv.

# Evaluation Metrics
The evaluation metric for this competition is Macro F-Score.
The F1 score, commonly used in information retrieval, measures accuracy using the statistics precision p and recall r. Precision is the ratio of true positives (tp) to all predicted positives (tp + fp). Recall is the ratio of true positives to all actual positives (tp + fn). The F1 score is given by:
F1= 2(p*r)/(p+r)   where p = tp/ (tp + fp) and r = tp/(tp + fn).

