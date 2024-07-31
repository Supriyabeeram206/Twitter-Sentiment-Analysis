# Twitter-Sentiment-Analysis

Overview

This project focuses on performing sentiment analysis on a substantial dataset of tweets to classify them as either positive or negative. Sentiment analysis, a technique in natural language processing (NLP), is used to determine the sentiment expressed in text. The project aims to build and compare several machine learning models for accurate sentiment classification.

Dataset

The dataset comprises 1.6 million tweets, each labeled as either positive or negative, with the following columns:

target: Sentiment label (0 for negative, 1 for positive)
id: Unique tweet identifier
date: Timestamp of the tweet
flag: Query flag (not used in this project)
user: Username of the tweet author
text: Content of the tweet
Libraries Used

numpy
pandas
re
nltk
scikit-learn
pickle
Preprocessing

Data Cleaning: Removed URLs, usernames, and non-alphabetic characters from tweets.
Stemming: Applied Porter Stemmer to reduce words to their root forms.
Stopwords Removal: Eliminated common English stopwords to minimize noise.
Feature Extraction

Utilized the TF-IDF vectorizer to convert the cleaned text into numerical features suitable for machine learning models.

Models

Trained and compared the following machine learning models: Logistic Regression and Random Forest. The models were evaluated based on their accuracy on both training and test datasets, with additional measurement of training and prediction times for performance comparison.

Results

Model evaluation results, including accuracy scores and training times, are detailed in the notebooks/model_comparison.ipynb notebook.

Future Work

Implement additional preprocessing techniques, such as lemmatization.
Incorporate emojis into sentiment analysis.
Acknowledgements

The dataset used in this project is provided by Kaggle and is publicly available ['https://www.kaggle.com/datasets/kazanova/sentiment140'].
