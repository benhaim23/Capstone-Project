# Bitcoin Price Forecasting and Sentiment Predictor Using Twitter Data, Google Trends and Technical Indicators

# Introduction
This project aims to forecast the price of Bitcoin and analyze sentiment related to Bitcoin on Twitter using machine learning techniques. The project utilizes historical Bitcoin price data, Google search trends for Bitcoin, and a large collection of tweets about Bitcoin to build predictive models.

# Project Organization
README.md          <- The top-level README for developers using this project.

SummaryReport_Bitcoin_Prediction_Analysis.pdf    <- Executive summary

Mark_Benhaim_Sprint1_presentation.pdf            <- Interim presentation of the project

Presentation_Bitcoin_Preidiction_Analysis.pdf    <- Final presentation of the project

# Notebooks:
Mark_Benhaim_Bitcoin_Prediction_Analysis_1_data_acquisition_cleaning.ipynb   <- Project notebook 1 - Data cleaning, preprocessing & EDA
Mark_Benhaim_Bitcoin_Prediction_Analysis_2_modelling.ipynb                   <- Project notebook 2 - modelling
Mark_Benhaim_Bitcoin_Prediction_Analysis_3_discussion.ipynb         <- Project notebook 3 - discussion

data (google drive link: (https://drive.google.com/drive/folders/1hJ4hLRzfGPtS2eAvBBD5uvXYwvAIQlDU?usp=sharing))
CSVs              

# Data
The project involves the following datasets:

1. Bitcoin Price Data: This dataset contains historical Bitcoin price data, including the opening price, closing price, volume, relative strength index (RSI), and historical volatility (HV).

2. Google Search Trends Data: This dataset includes Google search trends for the term "Bitcoin" over time.

3. Twitter Data: This dataset comprises a collection of tweets about Bitcoin. The tweets are preprocessed and cleaned to extract meaningful information.

# Data Cleaning
The project involved extensive data cleaning to prepare the datasets for analysis. The steps performed include:
1. Cleaning the Tweets Dataset: The tweets dataset was cleaned by converting the date format, dropping unneeded columns, converting text to lowercase, removing special characters, digits, and numbers, removing stopwords, and performing stemming.

2. Cleaning the Bitcoin Data: The Bitcoin price data was cleaned by handling missing values and converting relevant columns to the appropriate data types.

3. Cleaning the Trends Data: The Google search trends data was cleaned by converting the date format and removing duplicate rows.

# Data Visualization
Various data visualizations were created to gain insights into the datasets and better understand the relationships between different variables. The visualizations include line plots, box plots, pair plots, wordcloud and heatmaps.

# Feature Engineering
A new DataFrame was created extracted from the tweets data, focusing on the five most repeated keywords and their counts. Another variable was added to store the total count of all keywords for each date.

# Combining Datasets
The datasets were combined based on the date to create a new DataFrame that includes Bitcoin price data, Google search trends, and tweet counts for each date.

# Next Steps
The current progress of the project includes data cleaning, visualization, and feature engineering. The next steps for the project can be as follows:

1. Time-Series Analysis: Perform time-series analysis on the Bitcoin price data to identify trends, seasonality, and patterns. This can help in building more accurate forecasting models.

2. Sentiment Analysis: Conduct sentiment analysis on the tweets data to classify tweets as positive, negative, or neutral sentiment. This can provide valuable insights into the overall sentiment related to Bitcoin on Twitter.

3. Bitcoin Price Forecasting: Use the cleaned and combined dataset to build predictive models for forecasting Bitcoin prices. Explore various time-series forecasting techniques such as ARIMA, LSTM, or Prophet.

4. Sentiment Predictor: Develop a machine learning model to predict the sentiment of tweets about Bitcoin. This can be done using natural language processing (NLP) techniques and sentiment analysis libraries.

5. Feature Importance: Analyze the importance of different features in predicting Bitcoin prices and sentiment. This can provide insights into which variables have the most significant impact on the outcomes.

6. Model Evaluation and Deployment: Evaluate the performance of the forecasting and sentiment prediction models using appropriate metrics. Once the models are deemed accurate and reliable, they can be deployed for real-time predictions.

7. Interactive Dashboard: Create an interactive dashboard using tools like Plotly or Dash to visualize the forecasted Bitcoin prices, sentiment trends, and other relevant insights.

# Expected Outcomes and Impact: 

This study has the potential to reveal insights about the influence of public sentiment on Bitcoin prices. The predictive models built from this research could be beneficial to investors, providing a more holistic view of market conditions by incorporating public sentiment. This project also contributes to the broader field of study regarding the influence of social media on financial markets.

# License
This project is licensed under the [MIT License](LICENSE).

# Contact
For any inquiries or collaborations, please contact [Mark Benhaim](markbenhaim0@gmail.com)

# Acknowledgments
Special thanks to Kaggle, Tradingview, Google, Brainstation
