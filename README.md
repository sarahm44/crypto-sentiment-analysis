# Crypto Sentiment Analysis

## Overview

In this repository I applied natural language processing to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum. I also applied fundamental NLP techniques to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.

I completed the following tasks:

1. Sentiment Analysis
2. Natural Language Processing
3. Named Entity Recognition

## Sentiment Analysis

I used the [newsapi](https://newsapi.org/) to pull the latest news articles for Bitcoin and Ethereum and created a DataFrame of sentiment scores for each coin.

### Questions:

Q: Which coin had the highest mean positive score?

A: Ethereum

Q: Which coin had the highest compound score?

A: Ethereum had the highest mean compound score. Bitcoin had the highest max compound score.

Q. Which coin had the highest positive score?

A: Ethereum


## Natural Language Processing

In this section, I used NLTK and Python to tokenize text, find n-gram counts, and create word clouds for both coins. 

### Tokenize

I completed the following:

1. Changed each word to lowercase.
2. Removed punctuation.
3. Removed stop words.

#### N-grams

Then I looked at the ngrams and word frequency for each coin.

I completed as follows:
1. Used NLTK to produce the ngrams for N = 2.
2. Listed the top 10 words for each coin.

#### Word Clouds

Finally, I generated word clouds for each coin to summarize the news for each coin.

See Bitcoin word cloud:
![](https://github.com/sarahm44/crypto-sentiment-analysis/edit/main/images/btc_cloud.png)

See Ethereum word cloud:
![](https://github.com/sarahm44/crypto-sentiment-analysis/edit/main/images/eth_cloud.png)


## Named Entity Recognition

In this section, I built a named entity recognition (NER) model for both coins and visualized the tags using SpaCy.

See Bitcoin NER:
![](https://github.com/sarahm44/crypto-sentiment-analysis/edit/main/images/btc_ner.png)

See Ethereum NER:
![](https://github.com/sarahm44/crypto-sentiment-analysis/edit/main/images/btc_ner.png)
