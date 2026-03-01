# 🛒 Retail Customer Segmentation (RFM Analysis)

## 📌 Project Overview
This project takes a raw, real-world dataset of over 400,000 online retail transactions and builds a Customer Segmentation model using **RFM (Recency, Frequency, Monetary)** analysis. The goal of this project is to identify the highest-value customers so the marketing team can run targeted, data-driven campaigns.

## 🛠️ Tools & Libraries Used
* **Python & Pandas** (Data Cleaning, Feature Engineering, Aggregation)
* **Matplotlib & Seaborn** (Data Visualization)
* **Kaggle** (Dataset link: https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset)

## 🧹 The Data Pipeline
1. **Data Cleaning:** Removed missing Customer IDs, handled negative quantities (returns/refunds), and filtered out massive B2B wholesale outliers to protect the mathematical averages.
2. **Feature Engineering:** Created a "Snapshot Date" to calculate exactly how many days had passed since each customer's last purchase.
3. **Aggregation:** Grouped 400,000+ receipts down to 4,300 unique customers, calculating their individual Recency, Frequency, and Total Spend.
4. **Statistical Scoring:** Utilized `pd.qcut` to assign statistical percentile scores (1-4) to each customer, creating an overall `RFM_Score`.

## 📊 Key Insights & Business Recommendations
Based on the segmentation, I identified a core group of **"Champion"** customers. To maximize ROI, the business should:
* Collect emails from the Champions and offer them early access to deals before they are announced to the general public.
* Make the Champions the focal point of upcoming marketing strategies.
* Provide special loyalty discounts to ensure high-value customers stay hooked to the organization's services and products.
