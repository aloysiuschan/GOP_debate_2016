# GOP_debate_2016

The Jupyter notebook uses natural language processing and the multinomial Naive Bayes algorithm to predict the sentiments of tweets on the 2016 GOP presidential debate.

I first clean the tweets by removing non-alphabets, converting all words to lowercase, removing stopwords, and converting all words into their root form.

After cleaning the tweets, I use them to generate a bag-of-words model. I then split the data into training and test sets, fit a multinomial Naive Bayes model to the training set, and generate sentiment predictions on the test set.

The multinomial Naive Bayes model achieved a test accuracy of 82%, which is better than the baseline accuracy of 79% (79% of all tweets were negative). The model correctly identified 51% of the positive tweets in the test set, and 89% of the negative tweets in the test set.

The dataset was obtained from Crowdflower's "Data For Everyone" library (https://www.figure-eight.com/data-for-everyone/).
