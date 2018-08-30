# GOP_debate_2016

The Jupyter notebook is split into three parts.

Part 1 contains code to predict the sentiments of tweets about the GOP presidential debate 2016, via Naive Bayes classification. Prior to training the model, the text data is cleaned (e.g. by removing stopwords and punctuation).

Part 2 uses the AFINN lexicon to assign a sentiment value (between -5 and 5) to each word in a tweet; the sentiment values of the words are then summed to produce a sentiment value for the tweet itself. Sentiment value of the tweet is then used to classify the tweet as "Positive" or "Negative", and this classification is compared against the actual classification to evaluate the accuracy of the AFINN sentiment analysis method. Note that this method of sentiment analysis does not require the data to be split into training and test sets, since this method does not involve model training.

Part 3 uses the VADER sentiment analysis engine to assign sentiment values to tweets; VADER attempts to measure text sentiments accurately by accounting for valence shifters such as negations (for more details, refer to this paper by the creators of VADER: http://comp.social.gatech.edu/papers/icwsm14.vader.hutto.pdf). Sentiment value of the tweet is then used to classify the tweet as "Positive" or "Negative", and this classification is compared against the actual classification to evaluate the accuracy of VADER.

I find that the Naive Bayes classifier (88% accuracy on the training set, 78% accuracy on the test set) outperforms the AFINN sentiment analysis method (66% accuracy on the full dataset). Surprisingly, the AFINN method outperforms the VADER method (62% accuracy on the full dataset), despite the relative sophistication of the latter method.

The dataset is obtained from Crowdflower's "Data For Everyone" library (https://www.figure-eight.com/data-for-everyone/).
