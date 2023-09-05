# Bitcoin Price Forecasting and Sentiment Predictor Using Twitter Data, Google Trends and Technical Indicators

# Introduction
This project aims to forecast the price of Bitcoin and analyze sentiment related to Bitcoin on Twitter using machine learning techniques. The project utilizes historical Bitcoin price data, Google search trends for Bitcoin, and a large collection of tweets about Bitcoin to build predictive models.

# Data Dictionary
<img width="476" alt="Screenshot 2023-08-17 at 11 43 22 PM" src="https://github.com/benhaim23/Capstone-Project/assets/128685658/26f618af-e007-4247-8ead-2a892d3d385a">


# Project Organization
README.md          <- The top-level README for developers using this project.

SummaryReport_Bitcoin_Prediction_Analysis.pdf    <- Executive summary

Mark_Benhaim_Sprint1_presentation.pdf            <- Interim presentation of the project

Mark_Benhaim_Sprint2_presentation.pdf            <- Interim presentation of the project

Presentation_Bitcoin_Prediction_Analysis.pdf    <- Final presentation of the project

# Notebooks:
Mark_Benhaim_Bitcoin_Prediction_Analysis_1_data_cleaning_preprocessing_EDA.ipynb   <- Project notebook 1 - Data cleaning, preprocessing & EDA

Mark_Benhaim_Bitcoin_Prediction_Analysis_2_baseline_modelling.ipynb                   <- Project notebook 2 - baseline modelling

Mark_Benhaim_Bitcoin_Prediction_Analysis_3_Comprehensive_Model_Evaluation_and_Insights.ipynb  <- Project notebook 3 - Comprehensive Model Evaluation and Insights

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
We analyzed the importance of different features in our dataset in predicting Bitcoin prices and sentiment providing insights into which variables have the most significant impact on the outcomes. These variables are:
- Sentiment_Polarity_tweetcount
- bitcoin_tweetcount
- btc_tweetcount
- crypto_tweetcount
- cryptocurrency_tweetcount
- project_tweetcount
- total count
- Percent change in dominance (close/open)
- BTC Dominance Close
- Volume
- RSI (relative strength index)
- HV (historical volatility)

# Baseline Modelling
We began our modeling phase with a random forests regressor to capture more complex relationships in the data through the R^2 squared value and assess feature importance. We made several visualizations such as displaying the feature importance for the relevant features, a scatter plot to compare actual vs. predicted Bitcoin prices with a line of best fit to further assess the relationship between our models prediction vs actual Bitcoin price, and a temporal chart to visualize the accuracy of our prediction model relative to the actual price of Bitcoin.

# Comprehensive Model Evaluation and Insights
In this section, we delve deeper into the performance metrics of each model, providing a bird's-eye view of their predictive capabilities.

# Decision Tree Implementation
In this section, a Decision Tree model is implemented and assessed using scikit-learn. Decision Trees are versatile machine learning algorithms used for both classification and regression tasks. This section details the implementation of the Decision Tree Regressor and its evaluation.

# Neural Network Issues Explored
In this section, a Neural Network model is implemented using scikit-learn. Neural Networks are powerful models for capturing complex data relationships. The code outlines the development of an MLPRegressor model and its evaluation. We scrutinize the Neural Network model's limitations, hypothesizing its underperformance may be due to its inherent complexity, suboptimal hyperparameter settings, and most notably data size constraints due to limitations with our dataset.

# XGBoost Implementation
This section focuses on implementing and evaluating the XGBoost algorithm, a gradient boosting framework known for its efficiency and effectiveness. The code demonstrates the use of GradientBoostingRegressor with XGBoost and assesses its performance.

# Models Comparison and Assessment
This section conducts a comparative analysis of various regression models, including Decision Tree, Random Forest, XGBoost, and Neural Network. Key evaluation metrics such as R-squared, Mean Squared Error (MSE), and Mean Absolute Error (MAE) are calculated and compared to understand each model's predictive capabilities.

# K-Fold Cross-Validation Analysis
Beyond traditional evaluation, K-Fold Cross-Validation is conducted to ensure robust performance assessments. This iterative evaluation approach offers a more comprehensive view of the models' generalization capabilities. In this section, K-fold cross-validation is used to assess model performance across different subsets of the dataset. Four models (Random Forest, Decision Tree, XGBoost, and Neural Network) are evaluated, and their average R-squared scores are reported to gauge their generalization abilities.

# Final Takeaways and Recommendations
The concluding section synthesizes the findings, underscoring XGBoost's prowess in predicting Bitcoin prices with the highest R-Squared value. Random Forest also performs well, with a reasonably high R-squared score. However, the Neural Network model appears to underperform compared to other models, possibly due to its complexity, hyperparameter tuning, and data size considerations. Additionally, the significant correlations between features, especially Twitter sentiment data, and Bitcoin prices are highlighted. Recommendations are provided, suggesting traders and investors integrate such sentiment metrics to make more informed investment decisions.

# Overall Impact: 
This study has revealed insights about the influence of public sentiment on Bitcoin prices. The predictive models built from this research are beneficial to investors, providing a more holistic view of market conditions by incorporating public sentiment. This project also contributes to the broader field of study regarding the influence of social media on financial markets.

# License
This project is licensed under the [MIT License](LICENSE).

# Contact
For any inquiries or collaborations, please contact [Mark Benhaim](markbenhaim0@gmail.com)

# Acknowledgments
Special thanks to Kaggle, Tradingview, Google, Brainstation
