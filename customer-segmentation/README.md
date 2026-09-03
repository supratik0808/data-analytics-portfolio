# Customer Segmentation Analysis

Segmenting customers into actionable groups using clustering to support targeted marketing and retention strategy.

## 📌 Overview

This project analyzes a shopping trends dataset to identify distinct customer segments based on purchasing behavior, spending patterns, and loyalty indicators. The goal: move from a "one-size-fits-all" marketing approach to data-driven, segment-specific strategy.

## 🛠️ Tools Used

- **MySQL** — data cleaning, transformation, and querying
- **Orange Data Mining** — K-means clustering
- **Power BI** — segment visualization and interactive dashboard
- **Statistical validation** — ANOVA and box-plot analysis to confirm cluster separation

## 📊 Dataset

- 3,900 customer records with purchase history, spend amount, frequency, and demographic attributes

## 🔍 Methodology

1. **Data preparation** — cleaned and structured raw data in MySQL
2. **Clustering** — applied K-means clustering in Orange Data Mining to group customers by behavior
3. **Validation** — used ANOVA and box-plot analysis to statistically confirm the three-cluster solution was meaningful (not arbitrary)
4. **Visualization** — built an interactive Power BI dashboard to explore segment characteristics
5. **Reporting** — summarized findings and business recommendations in a final report and presentation

## 🎯 Key Results: Three Customer Segments

| Segment | Description |
|---|---|
| **New High-Spenders** | Recently acquired customers with high transaction values — high potential lifetime value |
| **Loyal Budget Shoppers** | Frequent, price-sensitive buyers — retain via value-driven offers |
| **VIP Loyal Customers** | Long-tenured, high-spend, high-frequency — priority for retention and loyalty programs |

## 📈 Dashboard

*(Add 2-3 Power BI screenshots here — e.g. `![Segment Overview](dashboard/segment_overview.png)`)*

## 📄 Full Report

See [`report/customer_segmentation_report.pdf`](report/customer_segmentation_report.pdf) for the complete analysis, statistical validation, and business recommendations.

## 💡 Business Impact

These segments enable targeted campaigns — e.g., loyalty rewards for VIP customers, value promotions for budget shoppers, and onboarding nurture flows for new high-spenders — rather than blanket marketing to the full customer base.
