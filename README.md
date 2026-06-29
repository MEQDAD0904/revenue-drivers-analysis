# E-Commerce Revenue Analysis

> ⚠️ **Note:** This was my first standalone analysis project.  
> It focuses on revenue patterns only — without customer behavior or business hypothesis.  
> A more complete and structured analysis is here:  
> 👉 ([https://github.com/MEQDAD0904/thelook-ecommerce-customer-retention-analysis-](https://github.com/MEQDAD0904/retention-revenue-connection))

---

## What This Project Is

An exploratory analysis of e-commerce transaction data focused on one question:

**What is driving revenue — order volume, order value, or both?**

No hypothesis framework was used here. This was early-stage exploration to understand the data before asking better business questions.

---

## What I Analyzed

- Revenue trends over time
- Order volume vs. average order value (AOV)
- Impact of high-value transactions (outliers) on total revenue
- Customer contribution to revenue
- Product contribution to revenue

---

## Dataset

| Table | Content |
|---|---|
| Orders | Transaction records |
| Order Items | Product-level detail per order |
| Products | Product catalog |

---

## Tools

- Python (Pandas, Matplotlib)
- Power BI

---

## Key Findings

**1. Revenue is volume-driven, not value-driven**  
Revenue trends followed order count closely. When orders dropped, revenue dropped. Price increases were not the growth engine.

**2. A small group of high-value transactions has outsized impact**  
~7.6% of transactions contributed ~34% of total revenue. Removing them stabilized AOV significantly.

**3. Revenue is spread across customers, not concentrated**  
~48,000 customers were needed to reach 80% of revenue — no strong VIP concentration at customer level.

**4. Products show more concentration than customers**  
~8,500 products generated 80% of revenue out of ~33,000 total. Product mix matters more than customer segmentation here.

**5. AOV is misleading without outlier context**  
With outliers: high and unstable. Without: lower and stable. Mean alone is not enough.

---

## What I Learned From This Project

This project showed me that analyzing revenue in isolation is incomplete.  
Revenue numbers don't explain themselves — they're the result of customer decisions, product performance, and order patterns working together.

This gap is what led me to build the next project:  
👉 ([https://github.com/MEQDAD0904/thelook-ecommerce-customer-retention-analysis-](https://github.com/MEQDAD0904/retention-revenue-connection))

---

## Project Files

| File | Description |
|---|---|
| `sales_analysis.py` | Data cleaning and analysis |
| `original_dashboard.png` | Main Power BI dashboard |
| `sales_dashboard_no_outliers.png` | Analysis without outliers |
| `sales_comparison.png` | Side-by-side comparison |

---

## How to Run

1. Load the datasets: `orders`, `order_items`, `products`
2. Run `sales_analysis.py`
3. Open the dashboard files to explore visuals
