# Adidas-Retail-Customer-Retention-Analytics-Power-BI Dashboard

This project focuses on customer churn, retention, repeat purchases, and customer lifetime value (CLV) analysis using transactional, customer, and store data. The goal is to build insightful Power BI dashboards to help business stakeholders make data-driven decisions.

## Tech Stack

- Power BI (data modeling, DAX, interactive dashboards)
- Power Query (ETL and data transformation)
- Excel (data exploration and validation)
- SQL (data extraction and aggregation)
- Python (optional advanced analysis and preprocessing)

## Dataset Overview

The analysis uses multiple datasets containing:

- Customer data: Region, Income Group, Age Group, Loyalty Tier, Membership_Since
- Transaction data: Transaction_Date, Amount, Channel (Store/Online), Product Category, Promotion_Flag
- Store data: Store_Type, Opening_Year, Location


## Tasks Performed

### Task 1: Data Modeling & Cleaning

- Loaded and transformed datasets in Power Query.
- Handled duplicates, missing values, and corrected data types.
- Created calculated columns:
  - `Membership_Duration = Today – Membership_Since`
  - Extracted `Transaction_Year` and `Transaction_Month`.

### Task 2: Churn & Retention Metrics

- Defined Churn Rate KPI:
  - `Churn Rate = (Churned Customers / Total Customers) * 100`
- Visualized churn rate by:
  - Region
  - Income Group
  - Channel (Store/Online)
  - Loyalty Tier
- Created a funnel view: **Total Customers → Repeat Customers → Churned Customers**.

### Task 3: Repeat Purchase Analysis

- Segmented customers by purchase count:
  - Low-Tier: 0–3 purchases
  - Mid-Tier: 4–8 purchases
  - High-Tier: 9+ purchases
- Compared average purchase frequency by Region, Age Group, and Loyalty Tier.
- Identified most purchased product categories by loyal customers.

### Task 4: Promotion & Loyalty Impact

- Calculated percentage of transactions with promotions applied.
- Compared average purchase amount with vs without promotions.
- Analyzed churn rate across loyalty tiers.
- Visualized **Points Earned vs Redeemed by Tier** using a clustered column chart.
- Derived recommendations to improve redemption and customer retention.

### Task 5: Store & Channel Performance vs Retention

- Merged store-level data with transaction data.
- Visualized:
  - Average transaction amount by Store Type.
  - Churn rate by Store Type.
  - Correlation between Store Opening Year and customer retention.

### Task 6: Customer Lifetime Value (CLV) Analysis

- Calculated CLV:
  - `CLV = Total Amount Spent / Membership Duration (Years)`
- Segmented customers into Low, Medium, and High CLV segments.
- Visualized:
  - CLV vs Days Since Last Purchase.
  - CLV by Loyalty Tier and Region.

### Task 7: Final Dashboard & Executive Summary

- Built a multi-page Power BI report:
  - Page 1: KPIs (Churn, CLV, Repeat Rate)
  - Page 2: Loyalty & Promotion Impact
  - Page 3: Store & Channel Insights
  - Page 4: Segmentation (Churned, Repeat, High-Value Customers)
- Added slicers for Region, Channel, Income Group, and Loyalty Tier.
- Summarized key business recommendations for Adidas:
  - Which customers to prioritize for retention.
  - Which channels are underperforming.
  - How to strengthen loyalty program engagement.


