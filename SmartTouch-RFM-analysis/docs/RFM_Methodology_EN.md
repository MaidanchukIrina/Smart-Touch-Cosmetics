# 📘 RFM Analysis Methodology

**Version:** 1.0  
**Date:** 27 Oct 2025  
**Department:** Smart Touch Marketing Analytics  
**Author:** Irina Maidanchuk  

---

## 🎯 Purpose of the RFM Analysis
RFM analysis is a classic customer segmentation technique used to evaluate **customer value and loyalty** based on purchasing behavior.  
It divides customers according to three key dimensions:

- **R (Recency)** – how recently a customer made a purchase  
- **F (Frequency)** – how often they purchase  
- **M (Monetary)** – how much they spend  

The purpose is to identify the most profitable and loyal clients, as well as those at risk of churn or in need of reactivation.

---

## 🧮 Key Metrics

| Metric | Meaning | Description |
|---------|----------|-------------|
| **Recency (R)** | Time since the last purchase | The shorter the time since last purchase, the higher the probability of retention. |
| **Frequency (F)** | Number of purchases | Reflects customer loyalty and engagement. |
| **Monetary (M)** | Total amount spent | Measures the financial value of the customer for the business. |

---

## 📊 Scoring Logic

Each indicator is assigned a **score (1–3 or 1–5)**, where:
- **3 or 5** = best performance  
- **1** = weakest performance  

### 🔹 Example of a 3-level scoring model:
| Score | Recency | Frequency | Monetary |
|--------|----------|------------|-----------|
| **3** | ≤ 6 months | > 10 orders | > 20,000 UAH |
| **2** | 6–24 months | 2–10 orders | 2,000–20,000 UAH |
| **1** | > 24 months | 1 order | < 2,000 UAH |

Each customer receives an RFM combination (e.g., `R=3, F=2, M=1`), forming the basis for segmentation.

---

## 🧩 Customer Segmentation by RFM

| Segment | Criteria | Description |
|----------|-----------|-------------|
| **VIP** | R > 6 mo, F > 10, M > 10K | Top-value clients who buy frequently and spend the most. |
| **Stable** | R ≤ 24 mo, M > 10K | Loyal and consistent buyers, slightly less active. |
| **Recent** | R ≤ 6 mo, medium F and M | Newly active or recently acquired clients. |
| **Monetary** | M > 10K, low R/F | Previously valuable, now inactive customers. |
| **Passive** | Low R, F, M | One-time or inactive customers. |

---

## 📈 Business Interpretation

| Segment | Marketing Actions |
|----------|-------------------|
| **VIP** | Retention programs, premium offers, personalized services. |
| **Stable** | Loyalty programs, cross-sell and re-engagement reminders. |
| **Recent** | Encourage repeat purchase via targeted campaigns. |
| **Monetary** | Reactivation campaigns (“win-back” discounts). |
| **Passive** | Low-priority group; mass or automated communication. |

---

## 📊 Typical Visualizations

1. **Treemap / Bar Chart** – revenue by RFM segment  
2. **Heatmap** – product preferences per group  
3. **Line / Area Chart** – revenue trend over time  
4. **Funnel Chart** – customer lifecycle stages  
5. **Scatter / Bubble Chart** – Recency vs Frequency vs Monetary

---

## 🧠 Use Cases in Smart Touch

RFM analysis is applied for:
- Personalizing offers in CRM  
- Predicting recurring revenue and churn  
- Prioritizing marketing efforts by customer segment  
- Understanding the customer lifecycle  
- Strategic planning for retention and upselling  

---

## ⚙️ Data Sources
- `clients.csv`  
- `sales.csv`  
- `rfm_scores.csv`  
- Data cleaned from duplicates, standardized date and currency formats.  
- Calculations executed in SQL/Python; visualization in Power BI / Tableau.

---

## 📁 Output Files
- `rfm_scores.csv` including:  
  `client_id`, `recency_score`, `frequency_score`, `monetary_score`, `rfm_group`, `revenue`, `orders_count`  
- Key visualizations for dashboard:
  - RFM Segmentation Overview  
  - Product Preferences by Segment  
  - Customer Lifecycle Funnel  

---

## 🧾 Update Recommendations
- Update frequency: **quarterly**  
- Automate refresh via Power BI or SQL jobs  
- Document any segmentation changes in `RFM_Methodology_EN.md`  

---

## 🏁 Conclusion
RFM analysis is a cornerstone of Smart Touch customer analytics.  
It provides a deep understanding of customer behavior, enables data-driven personalization, and supports sustainable business growth.

---
* |
