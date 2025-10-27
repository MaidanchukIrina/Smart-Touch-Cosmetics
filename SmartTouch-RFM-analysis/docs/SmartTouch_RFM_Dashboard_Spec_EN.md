
# Smart Touch — RFM Dashboard Specification (v2)

**Version:** 27.10.2025  
**Owner:** Marketing Analytics Department  
**Author:** Irina Maidanchuk  
**Reviewer:** Head of Marketing Analytics  

---

## 🎯 Business Goal
Visualize customer value and segmentation for Smart Touch to identify:
- High-value (VIP) and loyal customers  
- At-risk and inactive clients  
- Product preferences by segment and region  
- Dynamics of purchases and repeat behaviour  

The dashboard should support **marketing and business decisions** about retention, upselling, and regional campaigns.

---

## 🔍 Review of Current Dashboard
**Strengths**
- Clear RFM segmentation and revenue structure  
- Effective use of product heatmap for marketing insights  
- Clean color scheme  

**Improvements required**
1. Add **monthly trend of revenue and clients** split by RFM group  
2. Add **Repeat Purchase Rate** (≥2, ≥3, ≥4 orders)  
3. Add **Customer Lifecycle Funnel** (New → Active → Repeat → Loyal → Inactive)  
4. Add **geographical breakdown** (Top regions by clients & revenue)  
5. Add **filter panel** (period, RFM group, product category, region)  
6. Add **text box with business insights** (automatically or manually generated)

---

## 🧭 Dashboard Layout & Components

| # | Component | Description | Type |
|---|------------|-------------|------|
| 1 | **KPI Cards** | Total Clients · Total Revenue · Avg Check · Repeat Purchase Rate · Buy Rate (mo.) | Cards |
| 2 | **Revenue & Clients by RFM Group** | Compare revenue, clients count and LTV across segments | Combo bar + line |
| 3 | **Revenue Trend by Month (RFM split)** | Monthly revenue / clients trend per segment | Stacked area |
| 4 | **Repeat Purchase Rate** | % of clients with ≥2 / ≥3 / ≥4 orders | Horizontal bars |
| 5 | **Product Preferences by Segment** | % of clients who bought each product by RFM group | Heatmap |
| 6 | **Customer Lifecycle Funnel** | Distribution of clients along lifecycle stages | Funnel |
| 7 | **Geography** | Top 5 regions by revenue & clients | Map / dual-axis bar |
| 8 | **Key Insights Text Box** | Summary of findings for management | Text box |
| 9 | **Filters** | Period · RFM Group · Product Category · Region | Filter panel |

---

## ⚙️ Technical Notes
**Source tables**
- `clients.csv`
- `sales.csv`
- `rfm_scores.csv`
- `products.csv`
- `regions.csv`

**Key metrics**
- `Repeat Purchase Rate (2+)` = clients with ≥2 orders / total clients  
- `LTV` = total revenue / number of clients  
- `Buy Rate (mo.)` = average orders per month per client  

**RFM groups**  
VIP · Stable · Recent · Passive · Monetary

---

## 🎨 Design & Style Guide
- **Colors (Smart Touch palette):**
  - VIP — purple  
  - Stable — turquoise  
  - Recent — lilac  
  - Passive — gray  
  - Monetary — mint  
- Heatmap — pastel beige → green scale  
- Fonts — Open Sans / Segoe UI, regular weight  
- KPI cards — white background + large numbers  
- Keep a clean layout: max 7–8 visuals per page  

---

## 📁 Deliverables for Analyst
1. Updated Power BI file: `dashboard/SmartTouch_RFM_v2.pbix`  
2. 2 screenshots:  
   - `/dashboard/screenshots/main_dashboard.png`  
   - `/dashboard/screenshots/trend_by_month.png`  
3. Update `docs/SmartTouch_RFM_Dashboard_Spec.md` with implemented parts  
4. Create **Pull Request** titled `RFM Dashboard Update v2`  
5. In PR description, briefly note implemented KPIs and filters  

---

## 🗓️ Timeline
| Stage | Description | Deadline |
|-------|--------------|-----------|
| 1 | Implement dashboard updates | +3 days |
| 2 | Review by Marketing Analytics | +1 day |
| 3 | Fixes & final merge to main | +2 days |

---

## ✅ Expected Outcome
Final dashboard must:
- Present a complete view of client activity by RFM segments  
- Show revenue dynamics, repeat purchases, geography & product popularity  
- Be visually clear and decision-ready for management  
- Include intuitive filters and concise insight summary  

---
