# GOP_debate_2016

The Jupyter notebook is split into two parts.

Part 1 contains code to predict the sentiments of tweets about the GOP presidential debate 2016, via Naive Bayes classification. Prior to training the model, the text data is cleaned (e.g. by removing stopwords and punctuation).

Part 2 uses the AFINN lexicon to assign a sentiment value (between -5 and 5) to each word in a tweet; the sentiment values of the words are then summed to produce a sentiment value for the tweet itself. Sentiment value of the tweet is then used to classify the tweet as "Positive" or "Negative", and this classification is compared against the actual classification to evaluate the accuracy of the AFINN sentiment analysis method. Note that this method of sentiment analysis does not require the data to be split into training and test sets, since this method does not involve model training.

I find that the Naive Bayes classifier (88% accuracy on the training set, 78% accuracy on the test set) outperforms the AFINN sentiment analysis method (66% accuracy on the full dataset).

The dataset is obtained from Crowdflower's "Data For Everyone" library (https://www.figure-eight.com/data-for-everyone/).
