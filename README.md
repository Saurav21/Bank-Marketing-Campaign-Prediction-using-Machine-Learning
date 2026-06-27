# 🏦 Bank Marketing Campaign Prediction using Machine Learning



## 📌 Project Overview

Marketing campaigns are one of the most effective ways for banks to promote financial products such as **term deposits**. However, contacting every customer is both expensive and inefficient.

This project develops a **Machine Learning-based Customer Propensity Model** that predicts the likelihood of a customer subscribing to a term deposit. Customers are then ranked according to their predicted probability, allowing the bank to prioritize high-value prospects and significantly reduce campaign costs through **Gains and Lift Analysis**.

---

## 🎯 Business Objective

The primary objective of this project is to:

* Predict whether a customer will subscribe to a term deposit.
* Rank customers based on their probability of subscription.
* Optimize marketing campaigns by targeting only the most promising customers.
* Reduce campaign costs while maximizing conversion rates.

---

## 📊 Dataset

The dataset contains customer demographic information, financial attributes, previous marketing interactions, and campaign details.

### Features

| Category              | Features                                                      |
| --------------------- | ------------------------------------------------------------- |
| Customer Information  | Age, Job, Marital Status, Education                           |
| Financial Information | Balance, Housing Loan, Personal Loan, Credit Default          |
| Campaign Information  | Contact Type, Contact Month, Call Duration, Campaign Contacts |
| Previous Campaign     | Previous Contacts, Previous Outcome, Days Since Last Contact  |
| Target Variable       | Deposit Subscription (Yes/No)                                 |

---

## 🛠 Project Workflow

```
Data Collection
       │
       ▼
Exploratory Data Analysis
       │
       ▼
Data Preprocessing
       │
       ▼
Feature Encoding
       │
       ▼
Train-Test Split
       │
       ▼
Model Building
       │
       ▼
Hyperparameter Optimization
(RandomizedSearchCV)
       │
       ▼
Model Evaluation
       │
       ▼
Probability Prediction
       │
       ▼
Customer Ranking
       │
       ▼
Gains & Lift Analysis
       │
       ▼
Campaign Cost Optimization
```

---

## 📈 Exploratory Data Analysis

The exploratory analysis includes:

* Missing value analysis
* Distribution analysis
* Boxplots for outlier detection
* Correlation analysis
* Feature comparison by target class

### Outlier Treatment

The identified outliers were retained because they represent genuine customer behavior rather than data entry errors. Since the selected machine learning algorithms are tree-based models, which are robust to outliers, no outlier treatment was performed.

---

## ⚙️ Data Preprocessing

* Label Encoding for categorical variables
* Train-Test Split
* Target variable encoding

---

## 🤖 Machine Learning Models

The following tree-based models were evaluated:

* Decision Tree
* Random Forest
* Extra Trees
* XGBoost
* CatBoost
* LightGBM

Each model was optimized using **RandomizedSearchCV**.

---

## 📏 Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* Classification Report

---

## 📈 Customer Probability Ranking

The best-performing model predicts the probability of each customer subscribing to a term deposit.

Customers are then ranked from the highest to the lowest probability and divided into deciles.

This ranking enables targeted marketing campaigns instead of contacting every customer.

---

## 📊 Gains and Lift Analysis

The project includes:

* Gains Table
* Lift Table
* Gains Chart
* Lift Chart

These business evaluation techniques measure how effectively the model identifies potential subscribers compared to random targeting.

### Business Insight

The analysis demonstrates that a significant proportion of potential subscribers are concentrated within the top-ranked customer segments.

By targeting only the highest-ranked customers, the bank can substantially reduce marketing costs while maintaining a high conversion rate.

---

## 💻 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* XGBoost
* CatBoost
* LightGBM

---

## 📂 Repository Structure

```
Bank-Marketing-Campaign-Prediction/
│
├── data/
│   ├── bank.csv
│
├── images/
│   ├── banner.png
│   ├── gains_chart.png
│   ├── lift_chart.png
│
├── notebook/
│   ├── bank_marketing_campaign.ipynb
│
├── README.md
│
└── requirements.txt
```

---

## 🚀 Key Outcomes

* Built a customer propensity prediction model.
* Compared six tree-based machine learning algorithms.
* Optimized hyperparameters using RandomizedSearchCV.
* Generated customer probability scores for ranking.
* Developed Gains and Lift charts for campaign evaluation.
* Demonstrated how machine learning can improve marketing efficiency and reduce campaign costs.

---

## 📚 Skills Demonstrated

* Exploratory Data Analysis (EDA)
* Data Visualization
* Feature Engineering
* Machine Learning
* Hyperparameter Tuning
* Model Evaluation
* Customer Propensity Modeling
* Marketing Analytics
* Gains & Lift Analysis
* Business Intelligence

---

## ⭐ Future Improvements

* Deploy the model using Streamlit or Flask
* Perform feature importance analysis using SHAP
* Build an interactive dashboard
* Automate customer ranking for real-time campaigns

---

## 👤 Author

**Saurav Bhuyan**



---

⭐ *If you found this project useful, consider giving it a star!*
