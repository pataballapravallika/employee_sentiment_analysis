# Employee Sentiment Analysis – Final LLM Assessment

## Project Overview
This project analyzes employee email communications to evaluate sentiment,
engagement levels, employee rankings, and potential flight risk using
Natural Language Processing (NLP) and statistical modeling techniques.

The dataset provided was unlabeled and required sentiment inference,
exploratory analysis, and predictive modeling.

---

## Objectives
- Automatically label employee messages as **Positive**, **Negative**, or **Neutral**
- Perform Exploratory Data Analysis (EDA)
- Calculate monthly sentiment scores for each employee
- Rank employees based on sentiment scores
- Identify employees at flight risk using a rolling 30-day window
- Build a linear regression model to analyze sentiment trends

---

## Tasks Implemented
### 1. Sentiment Labeling
- Combined email **Subject** and **Body** for better context
- Used **VADER Sentiment Analyzer**
- Labels: Positive, Negative, Neutral

### 2. Exploratory Data Analysis (EDA)
- Dataset structure and missing value analysis
- Sentiment distribution visualization
- Monthly sentiment trend analysis

### 3. Monthly Employee Sentiment Scoring
- Positive = +1
- Negative = −1
- Neutral = 0
- Scores reset each month

### 4. Employee Ranking
- Top 3 Positive employees per month
- Top 3 Negative employees per month
- Sorted by score and employee identifier

### 5. Flight Risk Identification
- An employee is marked **Flight Risk** if they send **4 or more negative emails**
  within any **rolling 30-day window**, regardless of month boundaries

### 6. Predictive Modeling
- Linear Regression model using:
  - Message count
  - Average message length
- Model performance evaluated using **R² score** and **RMSE**

---

## Key Insights
- Repeated negative sentiment is a strong indicator of flight risk
- Monthly sentiment trends show noticeable fluctuations
- Regression model achieved a moderate fit (R² ≈ 0.66), indicating
  behavioral features influence sentiment trends

---
