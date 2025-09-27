# Sentiment Analysis with Machine Learning

## 📖 Project Overview
This project builds a **Sentiment Analysis** pipeline using machine learning to classify text (reviews, tweets, or comments) into sentiment categories (e.g., Positive, Negative, Neutral).  
It supports multiple datasets and provides both single-text and batch predictions.

## 🚀 Features
- Automatic dataset loading and preprocessing  
- Text cleaning (remove URLs, mentions, hashtags, special chars)  
- Exploratory Data Analysis (EDA) with class distribution & text length stats  
- Machine learning models: Logistic Regression, Naive Bayes, Linear SVC  
- Model tuning with GridSearchCV  
- Performance metrics: Accuracy, F1-score, Confusion Matrix  
- Save & load models with `joblib`  
- Predict single text inputs  
- Batch predictions from CSV  

## 🛠️ Installation
```bash
pip install -r requirements.txt

Required packages:
pandas
numpy
scikit-learn
matplotlib
wordcloud
imbalanced-learn

📂 Dataset

The notebook supports:
user_reviews.csv
Twitter_Data.csv
tweets.csv

It automatically detects text and label columns.
Make sure your dataset has:
A text column (e.g., text, tweet, review)
A label column (e.g., sentiment, label, category)

▶️ Usage

Run the Jupyter Notebook:

jupyter notebook project_2_.ipynb

Single Prediction
predict_text("I absolutely love this app!")
Batch Prediction
Upload a CSV with a column named text. The model will add a new column predicted_sentiment and export predictions.csv.

📊 Results

Models compared: Logistic Regression, Naive Bayes, Linear SVC
Best model: Linear SVC with TF-IDF (after hyperparameter tuning)
Metrics (example results):
Accuracy: ~0.85
Weighted F1-score: ~0.84
