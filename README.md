# Capstone-Project - Bitcoin Price Prediction and Sentiment Predictor Using Twitter Data

# Executive summary

The goal of this project is to analyze and predict Bitcoin price changes by integrating technical indicators and sentiment analysis of Twitter data. We aim to investigate the correlation between public sentiment and Bitcoin price, as well as to evaluate the potential of sentiment analysis as a factor in Bitcoin price prediction models.

Data: We leverage two main datasets in this study:

Bitcoin Market data: The data includes date, opening and closing prices, percent change in price, Bitcoin dominance (opening and closing), percent change in dominance, trading volume, relative strength index (RSI), and historical volatility. The dataset consists of daily Bitcoin market statistics from August 19th, 2017 to the present.

Twitter data: The dataset consists of over one million cleaned tweets related to Bitcoin, each with an associated date.
The sample was taken over a span of 72 days during the year 2021. The tweets dataset is sourced from kaggle.

Methods: Our approach combines data preprocessing, exploratory data analysis (EDA), sentiment analysis, and predictive modeling.

Demo videos:

1 minute YouTube demo ____________________

5 minute demo + project overview & discussion _______________________

Tableau Dashboard: _____________________

# Project Organization
README.md          <- The top-level README for developers using this project.

SummaryReport_Bitcoin_Prediction_Analysis.pdf    <- Executive summary
Presentation_Bitcoin_Preidiction_Analysis.pdf    <- Final presentation of the project

notebooks:
Mark_Benhaim_Bitcoin_Prediction_Analysis_1_data_acquisition_cleaning.ipynb   <- Project notebook 1 - Data cleaning
Mark_Benhaim_Bitcoin_Prediction_Analysis_2_EDA_preprocessing.ipynb           <- Project notebook 2 - EDA
Mark_Benhaim_Bitcoin_Prediction_Analysis_3_modelling.ipynb                   <- Project notebook 3 - modelling
Mark_Benhaim_Bitcoin_Prediction_Analysis_2_discussion.ipynb         <- Project notebook 4 - discussion

data (google drive link: __________________)
CSVs              

# Introduction
Bitcoin Price Prediction and Sentiment Predictor is a tool that combines Bitcoin market data, technical indicators, and sentiment analysis of over a million tweets to predict Bitcoin price changes. It harnesses the power of public sentiment expressed on Twitter, converting it into valuable insights that contribute to a comprehensive understanding of Bitcoin's price dynamics.

Bitcoin and other cryptocurrencies have made a substantial impact on the global financial landscape. They offer an alternative investment option with high volatility that can yield significant returns. However, the unpredictable nature of Bitcoin prices necessitates advanced predictive tools for potential investors. An integral part of this puzzle could be the sentiment expressed on social media platforms like Twitter, where millions of users share their opinions and predictions about Bitcoin every day.

People love discussing Bitcoin and other cryptocurrencies on Twitter because it allows them to share their insights, learn about new trends, and be part of a global community of crypto enthusiasts. Similarly, investors and traders look to Twitter and other social media platforms to gauge public sentiment, which can often reflect or even predict market movements.

Currently, there is a limited range of tools that comprehensively incorporate both technical indicators and social sentiment in predicting Bitcoin price. This is where Bitcoin Price Prediction and Sentiment Predictor steps in. By analyzing the Bitcoin market data alongside Twitter sentiment, this tool provides a nuanced perspective of the market, facilitating more informed decision-making for investors.

Our tool goes beyond conventional market statistics to tap into the collective wisdom of the crypto Twitter community, translating it into actionable insights. With this, users can understand the potential impacts of public sentiment on price changes and get a step ahead in their investment journey. It's a tool for anyone who wants to delve deeper into the complexities of the Bitcoin market or harness the power of social sentiment in their investment strategy.

# Data Download, Cleaning & Exploratory Data Analysis
Two datasets were utilized for this project. The Bitcoin market data, comprising technical indicators such as opening and closing prices, percent change in price, Bitcoin dominance, trading volume, relative strength index (RSI), and historical volatility was downloaded. The dataset, which contains daily Bitcoin market statistics, extends from August 18, 2017, to the present.

The second dataset includes over one million cleaned tweets related to Bitcoin, obtained using Twitter's API. Each tweet is associated with a specific date, allowing for temporal analysis and the opportunity to align the data with Bitcoin market indicators.

**The cleaning process of the market data involved handling missing values and converting time-based columns into a proper datetime format. For the tweets dataset, cleaning had been performed before we obtained it. However, some additional preprocessing was applied: conversion of date from Excel's format to datetime and assigning sentiment scores (polarity and subjectivity) for each tweet using the TextBlob library.**

**These sentiment scores were then aggregated by day to align with the Bitcoin market data, with the mean sentiment score for each day calculated. The Bitcoin market data and the aggregated tweets data were then merged based on the date column, creating a comprehensive dataset that includes both market statistics and sentiment analysis of Twitter data.**

During the exploratory data analysis (EDA) phase, we examined the trends, patterns, and potential relationships within the data. The EDA highlighted the features that were likely to be good predictors of Bitcoin price changes. Further, we investigated the correlation between various market indicators, the sentiment scores, and the Bitcoin price.

The cleaned and processed dataset provides a valuable resource for understanding the interplay between Bitcoin prices, market indicators, and public sentiment on Twitter. After preprocessing and EDA, the dataset was divided into a training set and a test set, ready to be used in the predictive modeling phase.

The final cleaned dataset constitutes daily Bitcoin market statistics and aggregated Twitter sentiment scores, presenting a nuanced perspective for understanding and predicting Bitcoin price changes.

# Expected Outcomes and Impact: 

This study has the potential to reveal insights about the influence of public sentiment on Bitcoin prices. The predictive models built from this research could be beneficial to investors, providing a more holistic view of market conditions by incorporating public sentiment. This project also contributes to the broader field of study regarding the influence of social media on financial markets.
