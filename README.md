# 📰 Fake and Real News Detection using NLP

## 📌 Problem Statement

The rapid spread of fake news across digital platforms poses serious risks to society, including misinformation, public panic, and erosion of trust in credible journalism. With the increasing volume of online content, it is no longer feasible to manually verify every news article. There is a strong need for an automated, data-driven solution that can accurately distinguish fake news from real news based on linguistic and textual patterns.

This project addresses this challenge by leveraging **Natural Language Processing (NLP)** and **Machine Learning** techniques to build an effective fake news classification system.

---

## 🎯 Project Objective

The main objectives of this project are to:

* Analyze linguistic and stylistic differences between fake and real news articles
* Engineer meaningful textual and linguistic features
* Train and evaluate multiple machine learning models
* Identify the best-performing model for fake news detection

---

## 🗂️ Dataset Overview

* **Classes:** Fake News vs Real News
* **Class Distribution:**

  * REAL: 3,171 articles
  * FAKE: 3,164 articles

🔹 The dataset is **well-balanced**, helping to prevent model bias toward a single class and improving the reliability of evaluation metrics.

---

## 🔍 Exploratory Data Analysis (EDA) Insights

Key observations from the dataset include:

* **Balanced Dataset:** Nearly equal distribution of fake and real news improves classification fairness.
* **N-gram Analysis:** Fake and real news show noticeable differences in frequently used words and phrases, revealing distinct linguistic patterns.
* **POS Tagging Insights:** While overall Part-of-Speech distributions are similar, subtle differences—particularly in adjective usage—provide useful signals for classification.

---

## 🛠️ Text Preprocessing

To prepare the text data for modeling, the following preprocessing steps were applied:

* Text cleaning (removal of punctuation, numbers, and special characters)
* Tokenization
* Stop word removal
* Lemmatization

✅ These steps significantly improved feature quality and model performance.

---

## ⚙️ Feature Engineering

Model performance benefited from a combination of traditional and custom-engineered features:

### 🔹 TF-IDF Features

* Capture the importance of words relative to documents
* Provide effective numerical representations of text

### 🔹 Sentiment Features

* **Polarity:** Measures emotional tone (negative to positive)
* **Subjectivity:** Measures factual vs opinion-based language

### 🔹 Linguistic Feature

* **Adjective Ratio (adj_ratio):**

  * Designed to capture writing style
  * Fake news tends to use more emotional or exaggerated language

📌 The inclusion of linguistic and sentiment features enhanced the model’s ability to differentiate between fake and real news.

---

## 🤖 Models Trained and Evaluated

| Model                | Accuracy | Precision | Recall | F1-Score |
| -------------------- | -------- | --------- | ------ | -------- |
| SVM                  | 0.9361   | 0.94      | 0.94   | 0.94     |
| HistGradientBoosting | 0.9266   | 0.93      | 0.93   | 0.93     |
| Random Forest        | 0.9163   | 0.92      | 0.92   | 0.92     |
| Logistic Regression  | 0.9163   | 0.91      | 0.92   | 0.92     |

---

## 🏆 Model Performance Insights

* **Support Vector Machine (SVM)** achieved the highest overall performance across all metrics.
* The strong performance of SVM suggests that a linear classifier can effectively separate fake and real news when rich engineered features are used.
* **HistGradientBoosting** also performed well, highlighting the potential of tree-based ensemble models for this task.

---

## ✅ Solution Summary

This project demonstrates that fake news detection can be effectively addressed using:

* Robust text preprocessing
* TF-IDF-based text representation
* Sentiment and linguistic feature engineering
* Carefully selected machine learning models

The final solution achieved **over 93% accuracy**, proving the effectiveness of combining textual, emotional, and stylistic cues in fake news classification.

---

## 🚀 Conclusion and Future Work

The results show that machine learning models—particularly SVM—can successfully identify fake news when supported by strong NLP feature engineering. Understanding linguistic patterns such as adjective usage and sentiment plays a key role in effective detection.

### 🔮 Future Improvements

* Analyze misclassified articles for deeper insights
* Experiment with word embeddings (Word2Vec, GloVe)
* Explore deep learning models (LSTM, CNN, Transformers such as BERT)
* Deploy the model as a web application or API

---

## 📌 Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* NLTK / SpaCy
* TF-IDF Vectorization
* Machine Learning Models (SVM, Random Forest, Gradient Boosting)

---

📢 *This project highlights the importance of NLP and feature engineering in combating misinformation in the digital age.*

