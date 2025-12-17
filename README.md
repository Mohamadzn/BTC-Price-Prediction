Bitcoin Price Prediction using Sentiment Analysis and Network Data
Overview
This project aims to predict Bitcoin prices by combining social media sentiment analysis with blockchain network metrics and market data. Unlike traditional financial models that rely solely on historical price data, this approach integrates qualitative data (Twitter sentiment) and quantitative trends (Google search volume, blockchain difficulty, hash rate, and gold prices) to create a comprehensive feature set for forecasting.

Key Features
Sentiment Analysis: Utilizes NLTK VADER (Valence Aware Dictionary and sEntiment Reasoner) to compute sentiment scores (Positive, Negative, Neutral, Compound) from millions of Bitcoin-related tweets.

NLP Pipeline: Includes extensive text preprocessing:

Text cleaning (removing URLs, handles, special characters).

Stopword removal.

Stemming (PorterStemmer).

Multi-Source Data Aggregation: Merges data from various distinct sources into a single time-series dataset:

Twitter: Sentiment polarity and sensitivity.

Google Trends: Search interest for "Bitcoin" and "BTC" (via pytrends).

Blockchain.info: Network Difficulty, Hash Rate, and Transaction Counts.

Yahoo Finance: Gold Spot Prices (via yahoofinancials).

Market Data: Historical Open/High/Low/Close (OHLC) and Volume data.

Deep Learning Ready: The data is processed and structured for training machine learning models (imported libraries include TensorFlow and Scikit-Learn).

Technologies Used
Python 3.x

Data Manipulation: pandas, numpy

Natural Language Processing: nltk, re

Machine Learning: tensorflow, sklearn

Data Visualization: matplotlib, seaborn

APIs & Data Fetching: pytrends, yahoofinancials, urllib

Data Sources
Bitcoin Tweets: A large dataset of historical tweets (processed from bitcoin-tweets-14m.zip).

Bitcoin Price Data: Historical price CSV (btc-price.zip).

Google Trends: Historical search interest data.

Blockchain Network: Real-time network stats via Blockchain.info API.

Commodities: Gold price data via Yahoo Finance.
