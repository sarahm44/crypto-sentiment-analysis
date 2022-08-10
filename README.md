# Crypto Sentiment Analysis

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/sentimental.jpeg)

## Table of Contents
- [Overview](#overview)
- [Sentiment Analysis](#sentiment-analysis)
  * [Bitcoin Sentiment](#bitcoin-sentiment)
  * [Ethereum Sentiment](#ethereum-sentiment)
- [Natural Language Processing](#natural-language-processing)
  * [Tokenize](#tokenize)
  * [N-grams](#n-grams)
  * [Word Clouds](#word-clouds)
  * [Named Entity Recognition](#named-entity-recognition)


## Overview

In this repository I applied natural language processing to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum. I also applied fundamental NLP techniques to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.

I completed the following tasks:

1. Sentiment Analysis
2. Natural Language Processing
3. Named Entity Recognition

See this contained in this [Jupyter Lab notebook](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/crypto_sentiment_1.ipynb).

## Sentiment Analysis

I used the [newsapi](https://newsapi.org/) to pull the latest news articles for Bitcoin and Ethereum and created a DataFrame of sentiment scores for each coin.

### Bitcoin Sentiment

I created the Bitcoin sentiment scores dataframe:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/btc_df.png)

See Bitcoin sentiment below:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/btc_sentiment.png)

### Ethereum Sentiment

I created the Ethereum sentiment scores dataframe:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/eth_df.png)

See Ethereum sentiment as follows:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/eth_sentiment.png)

Some observations include that:

* Ethereum had the highest mean positive score.
* Ethereum had the highest mean compound score.
* Bitcoin had the highest max compound score.

## Natural Language Processing

In this section, I used NLTK and Python to tokenize text, find n-gram counts, and create word clouds for both coins. 

### Tokenize

I used NLTK and Python to tokenize the text for each coin. I completed the following:

1. Changed each word to lowercase.
2. Removed punctuation.
3. Removed stop words.

See relevant code below:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/tokenize.png)

I then added the "Tokens" column of the tokenized text to the dataframe:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/tokens_df.png)

### N-grams

Then I looked at the ngrams and word frequency for each coin.

I completed as follows:
1. Used NLTK to produce the ngrams for N = 2.
2. Listed the top 10 words for each coin.

See below the count for ngrams for N = 2:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/ngrams.png)

See below the code and results for the top 10 words for each coin:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/top10.png)

### Word Clouds

Finally, I generated word clouds for each coin to summarize the news for each coin.

See Bitcoin word cloud:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/btc_cloud.png)

See Ethereum word cloud:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/eth_cloud.png)


### Named Entity Recognition

In this section, I built a named entity recognition (NER) model for both coins and visualized the tags using SpaCy.

See Bitcoin NER:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/btc_ner.png)

See Ethereum NER:

![](https://github.com/sarahm44/crypto-sentiment-analysis/blob/main/images/eth_ner.png)
