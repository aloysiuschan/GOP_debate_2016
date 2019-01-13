# GOP_debate_2016

The Jupyter notebook uses natural language processing and the AdaBoost algorithm to predict the sentiments of tweets on the 2016 GOP presidential debate.

I first clean the tweets by converting all words to lowercase, removing stopwords, and converting all words to their root form.

After cleaning the tweets, I use them to generate a bag-of-words model. I then split the data into training and test sets, fit an AdaBoost model to the training set, and evaluate the model's performance on the test set.

The AdaBoost model achieved a test accuracy of 84.3%, which is better than the baseline accuracy of 79.2% (79.2% of all tweets were negative). In an attempt to improve predictive accuracy, I optimize the hyperparameters of the AdaBoost model via random search. After 5 iterations of random search, the optimized AdaBoost model achieved a test accuracy of 84.9%, which is slightly better than the test accuracy of the unoptimized AdaBoost model.

The dataset was obtained from Crowdflower's "Data For Everyone" library (https://www.figure-eight.com/data-for-everyone/).
