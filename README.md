# Task-3-ecommerce-data-analysis-python
Targeted business analytics answering 8 business questions via groupby aggregations, time-series trends, and customer segmentation
# 📊 ecommerce-data-analysis-python
> **DecodeLabs Industrial Training Kit — Project 3**  
> Batch 2026 | Data Analytics Track
## 📌 Project Overview

This project moves from exploration into **targeted analytical problem-solving**. Acting as a Data Analyst at DecodeLabs, you are given specific business questions that must be answered with precision — using groupby aggregations, filtering logic, time-series breakdowns, and customer segmentation.

This is the bridge between raw data exploration and the final visualization stage, producing structured analytical outputs that support executive decision-making.
## 🎯 Objectives

- Answer specific business questions using grouped aggregations
- Perform time-series analysis (monthly, quarterly, yearly revenue trends)
- Segment customers by order behavior, payment method, and referral source
- Analyze coupon code effectiveness on order revenue
- Identify high-value products and underperforming segments
- Build reusable analytical functions for each business question
## 🗂️ Dataset

| Property | Detail |
|---|---|
| File | `Project1_Cleaned_Dataset.xlsx` |
| Records | 1,200 orders |
| Columns | 15 |
| Date Range | January 2023 – June 2025 |
## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core language |
| pandas | GroupBy, pivot tables, filtering |
| numpy | Aggregation helpers |
| matplotlib / seaborn | Supporting visuals |
| openpyxl | Export results to Excel |
## 📁 Project Structure
ecommerce-data-analysis-python/
│
├── data/
│   └── Project1_Cleaned_Dataset.xlsx   # Input dataset
│
├── outputs/
│   ├── monthly_revenue_summary.xlsx    # Time-series output
│   ├── product_performance.xlsx        # Product breakdown
│   └── customer_segments.xlsx         # Segmentation results
│
├── Project3_Data_Analysis.py           # Main Python script
├── requirements.txt
└── README.md


## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/ecommerce-data-analysis-python.git
cd ecommerce-data-analysis-python

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the analysis script
python Project3_Data_Analysis.py
## 🔑 Business Questions Answered

| # | Business Question | Method |
|---|---|---|
| 1 | What is the total and average revenue per product? | `groupby` + `agg` |
| 2 | How has monthly revenue trended from 2023 to 2025? | `resample` + time-series |
| 3 | Which payment method generates the highest average order value? | `groupby mean` |
| 4 | What percentage of orders use each coupon code? | `value_counts` + normalization |
| 5 | Which referral source drives the most revenue? | `groupby sum` |
| 6 | What is the order cancellation and return rate by product? | Filtered `groupby` |
| 7 | Do customers with more items in cart spend more? | Correlation + binning |
| 8 | What is the revenue contribution of each order status? | Pivot table |
## 📊 Selected Results`
Monthly Revenue (Sample):
  Jan 2023 : $38,450
  Jun 2024 : $52,110  ← Peak
  Mar 2025 : $41,200

Top Products by Revenue:
  1. Laptop   — $214,830
  2. Monitor  — $198,450
  3. Tablet   — $176,210

Coupon Effectiveness:
  SAVE10     — 42% of coupon orders, avg $1,180/order
  FREESHIP   — 31% of coupon orders, avg $980/order
  WINTER15   — 27% of coupon orders, avg $1,340/order

## 📤 Outputs

All analytical summaries are exported to the `outputs/` folder as Excel files, ready for stakeholder sharing or further visualization in Project 4.


