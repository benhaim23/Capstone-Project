# Bitcoin Price Forecasting and Sentiment Predictor Using Twitter Data, Google Trends and Technical Indicators

# Introduction
This project aims to forecast the price of Bitcoin and analyze sentiment related to Bitcoin on Twitter using machine learning techniques. The project utilizes historical Bitcoin price data, Google search trends for Bitcoin, and a large collection of tweets about Bitcoin to build predictive models.

# Data Dictionary
<img width="564" alt="Screenshot 2023-07-27 at 10 29 27 PM" src="https://github.com/benhaim23/Capstone-Project/assets/128685658/9dab787e-e491-4b2a-9fd4-df11870aabab">


# Project Organization
README.md          <- The top-level README for developers using this project.

SummaryReport_Bitcoin_Prediction_Analysis.pdf    <- Executive summary

Mark_Benhaim_Sprint1_presentation.pdf            <- Interim presentation of the project

Presentation_Bitcoin_Preidiction_Analysis.pdf    <- Final presentation of the project

# Notebooks:
Mark_Benhaim_Bitcoin_Prediction_Analysis_1_data_cleaning_preprocessing_EDA.ipynb   <- Project notebook 1 - Data cleaning, preprocessing & EDA

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
A new DataFrame was created extracted from the tweets data, focusing on the five most repeated keywords and their counts: bitcoin, btc, crypto, cryptocurrency and project. Another variable was added to store the total count of all keywords for each date by day.

# Combining Datasets
The datasets were combined based on the date to create a new DataFrame that includes Bitcoin price data, Google search trends, and tweet counts for each date. Since there were many null values in the tweets dataset, we used a 3 day moving average fo fill the null values when combining the datasets to include more pricing data in our analysis.

# Sentiment Analysis: 
A sentiment analysis was conducted on the tweets data to classify tweets as positive, negative, or neutral sentiment providing valuable insights into the overall sentiment related to Bitcoin on Twitter. A visualization was made to display the disparity of each classification.

# Feature Importance: 
We analyzed the importance of different features in our dataset in predicting Bitcoin prices and sentiment providing insights into which variables have the most significant impact on the outcomes.

# Baseline Modelling
We began our modeling phase with a random forests regressor to capture more complex relationships in the data through the R^2 squared value and assess feature importance. We made several visualizations such as displaying the feature importance for the relevant features, a scatter plot to compare actual vs. predicted Bitcoin prices with a line of best fit to further assess the relationship between our models prediction vs actual Bitcoin price, and a temporal chart to visualize the accuracy of our prediction model relative to the actual price of Bitcoin.

# Next Steps
The current progress of the project includes data cleaning, visualization, and feature engineering. The next steps for the project can be as follows:

1. Modeling with Other Algorithms:
Explore alternative machine learning models, like nearual networks and support vector machines, to compare their performances with the Random Forest model.

2. Time-Series Analysis: Perform time-series analysis on the Bitcoin price data to identify trends, seasonality, and patterns. This can help in building more accurate forecasting models.

3. Bitcoin Price Forecasting: Use the cleaned and combined dataset to build more advanced predictive models for forecasting Bitcoin prices. Explore various time-series forecasting techniques such as ARIMA, LSTM, or Prophet.

4. Model Evaluation:
Evaluate the performance of the forecasting and sentiment prediction models using appropriate metrics. Once the models are deemed accurate and reliable, they can be deployed for real-time predictions. Beyond just R-squared, consider other metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), or Root Mean Squared Error (RMSE). A combination of metrics can provide a more holistic view of the model's performance. 

5. Fine-Tune Model Parameters:
Utilize techniques like grid search, confusion matrix or random search to optimize hyperparameters for the model. This can significantly improve performance and predictive accuracy.

6. Cross-Validation:
Implement K-fold cross-validation to ensure that the model is not overfitting and can generalize well to unseen data.

7. Comprehensive Workflow:
Once various other models, evaluation metrics, and cross-validation strategies have been explored, combine these elements into a cohesive pipeline. This pipeline can be used for future predictions, making the entire process more streamlined and efficient.

8. Interactive Dashboard: Create an interactive dashboard using tools like Plotly or Dash to visualize the forecasted Bitcoin prices, sentiment trends, and other relevant insights.

# Expected Outcomes and Impact: 

This study has the potential to reveal insights about the influence of public sentiment on Bitcoin prices. The predictive models built from this research could be beneficial to investors, providing a more holistic view of market conditions by incorporating public sentiment. This project also contributes to the broader field of study regarding the influence of social media on financial markets.

# License
This project is licensed under the [MIT License](LICENSE).

# Contact
For any inquiries or collaborations, please contact [Mark Benhaim](markbenhaim0@gmail.com)

# Acknowledgments
Special thanks to Kaggle, Tradingview, Google, Brainstation
