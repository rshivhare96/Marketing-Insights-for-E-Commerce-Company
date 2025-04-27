# 🛒 Marketing Insights for E-Commerce Company

This project analyzes customer behavior and marketing strategies for an e-commerce company using a transactional dataset. We perform exploratory data analysis, customer segmentation, and predictive modeling to uncover actionable insights for improving marketing efficiency and targeting.

---

## 📊 Data

The dataset contains historical purchase data and customer demographics with the following features:

- **Customer Information**: Customer ID, Gender, Age, Region
- **Transactional Data**: Purchase Amount, Number of Purchases, Product Categories
- **Marketing Engagement**: Email Clicks, Ads Viewed, Campaign Response

### Key Data Insights

- Minimal missing values, handled during preprocessing.
- Purchase patterns vary notably with age group and gender.
- Higher ad viewership is associated with higher purchase frequency.
- Email engagement is a strong indicator of campaign response.

---

## 🤖 Machine Learning Tasks

### 🔍 Classification – Predicting Campaign Response

Used a `RandomForestClassifier` to predict whether a customer would respond to a marketing campaign based on their demographics and behavior.

| Metric      | Score |
|-------------|-------|
| Accuracy    | ~0.79 |
| F1-Score    | ~0.76 |

✅ The classifier achieved good performance, showing strong relationships between customer features and marketing responsiveness.

---

### 🔢 Regression – Predicting Purchase Amount

Applied a `RandomForestRegressor` to predict customer purchase amounts using engagement and demographic features.

- **Mean Absolute Error (MAE)**: ~62.7
- **R² Score**: ~0.65

📈 Regression results show decent predictive ability, suggesting purchase amounts can be reasonably estimated using behavioral data.

---

## 🔗 Clustering – Customer Segmentation

### K-Means Clustering

Segmented customers into 4 distinct groups:

| Cluster | Traits |
|---------|--------|
| 0 - High Value Shoppers | High purchase amount, high engagement with ads and emails |
| 1 - Casual Buyers       | Moderate purchase behavior, low marketing interaction   |
| 2 - Price Sensitive     | Lower purchase amounts, moderate ad views               |
| 3 - Highly Engaged Non-Buyers | High ad and email interaction, lower actual purchases |

- **Silhouette Score**: ~0.49 — indicates reasonable cluster separation.

---

## 🔍 Notable Findings

- Customer engagement metrics (like email clicks and ad views) are critical predictors for both purchase behavior and campaign success.
- High-value customer segments can be specifically targeted with tailored promotions.
- Younger customers tend to engage more frequently but have more variable purchase behavior.
- Clustering provides actionable customer segments for personalized marketing strategies.

---

## 📁 Notebooks

[Marketing_Insights_for_E-Commerce_Company.ipynb](./Marketing%20Insights%20for%20E-Commerce%20Company.ipynb):  
Complete workflow including EDA, machine learning, and customer segmentation.

---

## 🛠 Requirements

To install the necessary libraries, run:

```bash
pip install -r requirements.txt
