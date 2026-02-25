# High-Value-Customer-Classification-Model
This project builds a supervised machine learning model to predict whether a customer is a high-value spender based on demographic and purchasing behavior features.  The objective is to help businesses proactively identify high-revenue customers and design targeted marketing strategies to maximize retention and profitability.End‑to‑end Data Science project: Exploratory Data Analysis ➜ Feature Engineering ➜ Classification Modeling ➜ Model Comparison

## 📌 Project Overview

This project analyzes customer purchasing behavior and builds a machine learning model to identify high‑spending customers. The pipeline includes data cleaning, visualization, statistical analysis, feature engineering, and predictive modeling.

### Business Goal:

Enable targeted marketing, personalized promotions, and revenue optimization by predicting customers likely to spend above average.

## 📊 Key Questions Answered

How does spending vary across gender?

Are there seasonal patterns in purchase amounts?

Do discounts significantly affect spending?

Which features most influence high spending?

Can we accurately classify high‑value customers?

## 🔎 Exploratory Data Analysis (EDA)
1️⃣ Spending Distribution by Gender

- Visualized using boxplots

- Shows spread, median, and outliers

- Helps detect demographic purchasing differences

2️⃣ Seasonal Sales Distribution

- Identifies peak spending seasons

- Mean markers highlight average spending differences

3️⃣ Impact of Discounts

- Compares spending with vs without discounts

- Useful for pricing and promotion strategies

4️⃣ Correlation Heatmap

- Displays relationships among numerical variables

- Detects multicollinearity and predictive signals

  ## 🏗️ Feature Engineering
##### Customer Lifetime Spend

Total spend per customer

### High‑Spender Label

Customers spending above the dataset mean are labeled as high spenders.

## 🤖 Machine Learning Models

| Model | Type | Key Strengths | Why Used in This Project |
|--------|------|--------------|---------------------------|
| Random Forest | Ensemble (Tree-based) | Handles non-linear data, robust to overfitting, provides feature importance | Main predictive model for identifying high spenders |
| Logistic Regression | Linear Classifier | Fast, interpretable, strong baseline | Used as benchmark model for comparison |

Data Split

Train: 80%

Test: 20%

Random state: 42

## Handling Class Imbalance

Random Forest configured with:

class_weight = 'balanced'

## 📈 Model Evaluation Metrics

Metrics used:

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| Random Forest | 0.91 | 0.89 | 0.93 | 0.91 |
| Logistic Regression | 0.85 | 0.82 | 0.87 | 0.84 |

These metrics provide a balanced evaluation for classification tasks, especially with imbalanced classes.

##  🏆 Best Model: Random Forest

Random Forest outperformed Logistic Regression in all evaluation metrics, making it the final model for high-spender prediction.

Key reasons:

- Captures non-linear relationships
- Robust to noise and outliers
- Handles feature interactions effectively
- Provides feature importance insights

## ⭐ Feature Importance Analysis

Top predictors identified using Random Forest feature importances.

Helps answer:

✔ What drives high spending?

✔ Which variables matter most for targeting?


## 🛠️ Tech Stack
Programming Language

Python 3.x

Libraries

pandas — data manipulation

numpy — numerical computing

matplotlib — visualization

seaborn — statistical plots

scikit‑learn — machine learning

## 📂 Project Structure

## 📂 Project Structure

```text
High-Value-Customer-Classification-Model/
│
├── Data Science Project.ipynb
├── customer_shopping.csv
├── README.md
│
└── images/
    ├── gender_spending.png
    ├── seasonal_sales.png
    ├── discount_impact.png
    ├── correlation_heatmap.png
    └── model_comparison.png
```

## 💡 Business Applications

Targeted marketing campaigns

Customer segmentation

Personalized discounts

Revenue forecasting

Churn prevention strategies

## 👨‍💻 Author

Jiya Jain
B.Tech — AI & ML
Aspiring Data Analytics and Data Scientist

