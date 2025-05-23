# Twitter Sentiment Analysis

This project performs **sentiment classification** on Twitter data using **Logistic Regression** and **Naive Bayes**. It applies natural language processing (NLP) and machine learning techniques to classify tweets into sentiments like `Positive`, `Negative`, `Neutral`, or `Irrelevant`.

---

## Dataset

The dataset is sourced from [Kaggle](https://www.kaggle.com/), containing:

- `twitter_training.csv` – training set
- `twitter_validation.csv` – validation set

Each row contains:
- Tweet ID
- Topic
- Sentiment label (`Positive`, `Negative`, `Neutral`, `Irrelevant`)
- Tweet text

---

## Tech Stack

- Python (Jupyter Notebook)
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn (TF-IDF, Logistic Regression, Naive Bayes)
- NLP (Text cleaning, tokenization, vectorization)

---

## Pipeline Overview

### 1. Data Preprocessing
- Cleaned tweets: removed URLs, mentions, hashtags, digits, and punctuation.
- Converted text to lowercase
- Encoded sentiment labels to integers

### 2. Feature Engineering
- Used `TfidfVectorizer` to transform text into numerical vectors

### 3. Model Training
- Trained two models:
  - **Logistic Regression**
  - **Multinomial Naive Bayes**

### 4. Evaluation
- Computed **Top-1 Accuracy**
- Visualized **Confusion Matrix**
- Compared model performance with **bar charts**
- Performed **GridSearchCV** to tune Logistic Regression's `C` parameter

---

## Results

- Achieved competitive accuracy using both models
- Logistic Regression accuracy improved through hyperparameter tuning
- Clear visualization of model predictions using Seaborn heatmaps

---



## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/twitter-sentiment-analysis.git
   cd twitter-sentiment-analysis
