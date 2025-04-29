# 📊 Customer Segmentation using RFM Analysis

## 🔍 Overview

This project applies **RFM (Recency, Frequency, Monetary) Analysis** to segment customers based on their purchase behavior. It's a smart way to identify high-value customers, inactive ones, and plan targeted marketing strategies.

---

## 📁 Dataset

- **Source:** Simulated customer data (1,000 records)
- **Fields Included:**
  - `Customer ID`, `Name`, `Email`, `Subscription Date`
  - Simulated:
    - `LastPurchaseDate` (randomized from Jan 2023 – Apr 2024)
    - `TotalPurchases` (Frequency)
    - `TotalSpend` (Monetary)

---

## ⚙️ Technologies Used

- Python
- Pandas, NumPy
- (Optional) Matplotlib, Seaborn
- Jupyter Notebook / Kaggle

---

## 🧠 Key Concepts

- **Recency:** How recently a customer purchased
- **Frequency:** How often they purchase
- **Monetary:** How much they spend

---

## 📌 Steps Performed

1. **Data Loading**
   - Loaded and explored the dataset using Pandas

2. **Feature Simulation**
   - Generated realistic values for `LastPurchaseDate`, `TotalPurchases`, and `TotalSpend` using NumPy

3. **RFM Metric Calculation**
   - Calculated Recency as the days since the last purchase
   - Used Frequency and Monetary values as simulated

4. **Scoring**
   - Used `pd.qcut()` to assign scores (1–5) for each R, F, M metric:
     - Lower `Recency` = higher score
     - Higher `Frequency` = higher score
     - Higher `Monetary` = higher score

5. **RFM Score Combination**
   - Combined `R_Score`, `F_Score`, and `M_Score` to generate a single RFM score like `555`, `431`, etc.

6. **Customer Segmentation**
   - Based on RFM_Score, segmented customers as:
     - `Champions`, `Loyal Customers`, `At Risk`, `Need Attention`, etc.

---

## 🧩 Sample Output

| Customer ID | Recency | Frequency | Monetary | R_Score | F_Score | M_Score | RFM_Score | Segment     |
|-------------|---------|-----------|----------|---------|---------|---------|-----------|-------------|
| 1001        | 8       | 9         | 4000     | 5       | 5       | 5       | 555       | Champion    |
| 1040        | 88      | 2         | 300      | 1       | 2       | 2       | 122       | At Risk     |

---

## 🎯 Why This Project Matters

- Real-world business application
- Teaches scoring and segmentation logic
- Builds strong data manipulation and analysis skills
- Easily extendable to dashboards (Power BI, Tableau)

---

## 🔄 Future Enhancements

- Create an interactive dashboard in Power BI
- Use real-world transactional data
- Apply clustering or ML for deeper analysis

---

> **Made as part of a hands-on learning journey to become a smart and skilled Data Analyst.**
