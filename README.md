# 🌍 Climate Change Tweet Analysis with Machine Learning & NLP

This project explores over **100,000 climate change-related tweets** using Natural Language Processing (NLP), Machine Learning, and data visualization techniques to uncover patterns in sentiment, stance, and public discourse.

## 📌 Project Objectives

- Classify tweets based on stance (Pro, Neutral, Anti) using supervised learning models.
- Forecast temperature trends using regression.
- Identify clusters in tweet behavior via unsupervised learning.
- Generate actionable insights from environmental and social data.

---

## 🗃️ Dataset Overview

- **Source**: Kaggle / Research Dataset
- **Size**: 100,000+ rows
- **Features**: 
  - `gender`, `sentiment`, `stance`, `aggressiveness`
  - `avg_temp`, `topic`, `country`, `disaster_event`
  - Temporal (`year`, `month`, `day`)

---

## ⚙️ Data Processing

### 🧹 Data Wrangling

- Removed duplicates and nulls
- Label encoded categorical features
- Applied scaling using `StandardScaler` and `ColumnTransformer`
- PCA used for dimensionality reduction where applicable

---

## 📊 Descriptive & Diagnostic Analysis

- Sentiment distribution showed majority positive or neutral tweets.
- Most users exhibited a **pro-climate change** stance.
- Geographic & temporal plots highlighted spikes during major climate events.
- Correlations identified between **stance**, **temperature deviation**, and **topics** discussed.

---

## 🔍 Predictive Modeling

### ✅ **Stance Classification**

| Model                | Accuracy  |
|---------------------|-----------|
| Logistic Regression | 72.2%     |
| SVM                 | 72.2%     |
| KNN                 | 72.0%     |
| Naive Bayes         | 71.9%     |
| Random Forest       | 69.5%     |

- Evaluation Metrics: **Precision**, **Recall**, **F1-Score**, **Confusion Matrix**, **ROC Curve**

### 📈 **Temperature Forecasting**
- Used **Linear Regression**
- Result: Poor fit (R² = -0.037)
- Recommendation: Use **ARIMA**, **Prophet**, or **LSTM** for seasonality

### 🌀 **K-Means Clustering**
- Features: Sentiment, Temperature, Encoded Topic
- PCA + Elbow Method selected **k = 4**
- Revealed distinct user behavior clusters

---

## 📌 Key Insights

- Stance prediction models perform well with moderate accuracy
- Clustering reveals distinct patterns in tweet behavior and concern
- Temperature dynamics require advanced modeling techniques
- Sentiment and topic distributions can guide communication strategies

---

## 🧠 Recommendations

- Use advanced time series models for climate forecasting
- Deploy targeted messaging based on stance clusters
- Monitor topic-wise trends in real time for public outreach
- Retrain classification models periodically with new tweets
- Integrate tweet sentiment with real-world climate events

---

## 🛠️ Tools & Libraries Used

- **Languages**: Python
- **Libraries**:
  - `pandas`, `numpy`, `matplotlib`, `seaborn`
  - `scikit-learn`, `xgboost`
  - `nltk`, `PCA`, `KMeans`, `Prophet`, `ARIMA`

---

## 📁 Repository Structure


