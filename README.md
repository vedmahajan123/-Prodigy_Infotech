📌 Sentiment Analysis & Visualization of Social Media Data
📖 Project Overview

This project performs sentiment analysis on Twitter data to understand public opinion and attitudes towards topics and brands.
We use machine learning (Logistic Regression) and text visualization to identify sentiment patterns in tweets.

The goal is to analyze how people feel (Positive, Negative, Neutral, Irrelevant) and visualize these insights with graphs and word clouds.

📂 Dataset

Files Used:

  twitter_training.csv

  twitter_validation.csv

Columns:

  id → Tweet ID

  entity → Topic/brand being discussed

  sentiment → Sentiment label (Positive, Negative, Neutral, Irrelevant)

  text → Tweet content

⚙️ Steps in the Project

1) Load Data

 Read Twitter datasets into Pandas.

2) Preprocessing & Cleaning

 Remove URLs, mentions (@user), hashtags, punctuation.
 Convert text to lowercase.
 Fill missing values.

3) Feature Extraction

  Use TF-IDF Vectorizer (top 5000 words) to convert tweets into numerical vectors.

4) Model Training

 Train a Logistic Regression classifier on training data.

5) Evaluation

  Accuracy score.

  Classification report (precision, recall, F1).

  Confusion matrix heatmap.

6) Visualization

  Sentiment distribution (bar chart).

  Word Clouds for Positive, Negative, Neutral tweets.

📊 Results

Accuracy: ~80–85% (varies by dataset split).

Insights:

  Positive tweets contain words like “love, great, happy”.

  Negative tweets highlight “bad, hate, worst”.

  Neutral tweets often contain factual statements.

-- Most errors happen between Neutral and Irrelevant tweets (because their language overlaps).
