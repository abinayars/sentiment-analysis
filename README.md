# Sentiment Analysis using Machine Learning

## Overview

This project is a machine learning-based sentiment analysis system that classifies text into **Positive** and **Negative** sentiment.

The project uses the **Sentiment140 Twitter dataset** for training and evaluation. Text data is cleaned and transformed into numerical features using **TF-IDF**, followed by classification using Logistic Regression and Multinomial Naive Bayes.

## Features

- Text preprocessing and cleaning
- Stopword removal
- TF-IDF feature extraction
- Logistic Regression classification
- Multinomial Naive Bayes classification
- Model comparison
- Accuracy, precision, recall and F1-score evaluation
- Confusion matrix analysis
- New-text sentiment prediction
- Cross-domain evaluation using IMDb movie reviews
- Trained model persistence using Joblib

## Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Jupyter Notebook
- Joblib

## Dataset

The primary dataset used is the **Sentiment140 Twitter dataset**.

- Training samples: 158,434
- Testing samples: 39,609

An IMDb dataset containing **10,000 movie reviews** was additionally used to evaluate cross-domain performance.

## Machine Learning Models

Two classification algorithms were implemented and compared:

1. Logistic Regression
2. Multinomial Naive Bayes

### Model Performance

| Model | Accuracy |
|---|---:|
| Logistic Regression | 76.53% |
| Multinomial Naive Bayes | 75.80% |

Logistic Regression achieved the higher accuracy on the Twitter test dataset.

## Cross-Domain Evaluation

The trained Logistic Regression model was additionally evaluated on IMDb movie reviews.

**IMDb Accuracy: 70.84%**

This evaluation demonstrates how the model performs when applied to text from a different domain.

## Evaluation Metrics

The selected model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Model Persistence

The trained model and TF-IDF vectorizer were saved using Joblib:

- `sentiment_model.pkl`
- `tfidf_vectorizer.pkl`

These files allow the trained components to be loaded later without retraining the model.

## Project Structure

```text
sentiment-analysis/
│
├── sentiment_analysis.ipynb
├── sentiment_model.pkl
├── tfidf_vectorizer.pkl
└── README.md
