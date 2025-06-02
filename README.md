#  Predicting High Value Users from Google Analytics BigQuery Data

This project builds an end-to-end machine learning pipeline to predict **high-value users** based on their behavior in Google Analytics session data.

We use the **Google Analytics Sample Sessions** public BigQuery dataset:
- [`bigquery-public-data.google_analytics_sample.ga_sessions_20170801`](https://console.cloud.google.com/marketplace/product/bigquery-public-data/google-analytics-sample)

---

##  Project Pipeline

✅ Load 20,000 Google Analytics session records from BigQuery  
✅ Data cleaning & feature engineering  
✅ Aggregate user-level behavioral features  
✅ Define **target variable**: high-value user (top 20% by pageviews)  
✅ One-hot encode categorical features  
✅ Train/test split (70/30)  
✅ Train classification models:
- RandomForest
- XGBoost  
✅ Evaluate models:
- Classification report
- ROC AUC score
- Confusion Matrix
- Feature Importance
- Precision-Recall curve

---

##  Dataset

Google Analytics Sample Sessions (BigQuery Public Dataset):
- 20,000 sessions for 1 day: `2017-08-01`
- Features used:
    - Pageviews
    - Hits
    - Visits
    - Channel Grouping
    - Country
    - Device Browser
    - Operating System
    - Traffic Source / Medium

---

##  Model Results

| Model | Accuracy | ROC AUC | Precision (Class 1) | Recall (Class 1) | F1-score (Class 1) |
|-------|----------|---------|--------------------|-----------------|-------------------|
| RandomForest | 98% | 0.999 | 1.00 | 0.89 | 0.94 |
| XGBoost      | 97% | 0.998 | 0.95 | 0.91 | 0.93 |


---

##  Visualizations Included

✅ Class Balance Plot  
✅ Feature Importance (RandomForest + XGBoost)  
✅ Confusion Matrix  
✅ ROC Curve (both models)  
✅ Precision-Recall Curve (XGBoost)  

---

##  How to Run

1️⃣ Open in Google Colab: [https://colab.research.google.com/](https://colab.research.google.com/)  
2️⃣ Copy code from `Google_Analytics_BigQuery.ipynb`  
3️⃣ Authenticate Colab → BigQuery  
4️⃣ Run notebook end-to-end  
5️⃣ All visualizations + model results will appear

---

##  Technologies Used

- Google BigQuery
- Google Colab
- Python 3
- pandas
- matplotlib
- seaborn
- scikit-learn
- xgboost


---

##  Project Highlights

✅ Real-world dataset — no synthetic data  
✅ Direct BigQuery → Colab pipeline  
✅ End-to-end supervised learning project  
✅ Clean ML pipeline:
- Data → Features → Modeling → Evaluation → Visualization 

---


