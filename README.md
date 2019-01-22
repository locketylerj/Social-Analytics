Distinguishing Sentiments

## Background

**Twitter** has become a wildly sprawling jungle of information—140 characters at a time. Somewhere between 350 million and 500 million tweets are estimated to be sent out _per day_. With such an explosion of data, on Twitter and elsewhere, it becomes more important than ever to tame it in some way, to concisely capture the essence of the data.


## News Mood

This Python script performs a sentiment analysis of the Twitter activity of various news outlets, and presents the findings visually.

The final output is a visualized summary of the sentiments expressed in Tweets sent out by the following news organizations: **BBC, CBS, CNN, Fox, and New York times**.

The first plot will be and/or feature the following:

* Be a scatter plot of sentiments of the last **100** tweets sent out by each news organization, ranging from -1.0 to 1.0, where a score of 0 expresses a neutral sentiment, -1 the most negative sentiment possible, and +1 the most positive sentiment possible.
* Each plot point will reflect the _compound_ sentiment of a tweet.
* Sort each plot point by its relative timestamp.

The second plot will is a bar plot visualizing the _overall_ sentiments of the last 100 tweets from each organization. This plot is an aggregate of the compound sentiments analyzed by VADER.

The tools used for this script include the following: tweepy, pandas, matplotlib, and VADER.

The Jupyter notebook:

* Pulls last 100 tweets from each outlet.
* Perform a sentiment analysis with the compound, positive, neutral, and negative scoring for each tweet.
* Pulls into a DataFrame the tweet's source account, its text, its date, and its compound, positive, neutral, and negative sentiment scores.
* Exports the data in the DataFrame into a CSV file.
* Saves PNG images for each plot.

* Also included is a written description of three observable trends based on the data.

