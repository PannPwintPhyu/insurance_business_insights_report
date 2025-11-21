# insurance_business_insights_report
Welcome to the **Insurance Business Insights** project 🚀   End-to-end SQL + Power BI analytics solution designed to transform operational insurance data into actionable business insights.

This project showcases my practical BI skillset across data modeling, ETL design, business logic implementation, and storytelling using an optimized analytical data warehouse.

---

## 🔗 Live Power BI Dashboard

➡️ **View Interactive Report**
[https://app.powerbi.com/view?r=eyJrIjoiMDdkNzA2ZWYtODBkZC00ZGYwLWIzZTgtNmNkNTdjODVmMmFjIiwidCI6IjIyODhlZGEwLWZiMTQtNDVlZS05OTY2LWE4ZGIwNDY2YzUzOSIsImMiOjEwfQ%3D%3D](https://app.powerbi.com/view?r=eyJrIjoiMDdkNzA2ZWYtODBkZC00ZGYwLWIzZTgtNmNkNTdjODVmMmFjIiwidCI6IjIyODhlZGEwLWZiMTQtNDVlZS05OTY2LWE4ZGIwNDY2YzUzOSIsImMiOjEwfQ%3D%3D)

---

## 📊 Dashboard Preview

*(Insert images here)*

* **Main Dashboard**
* **Customer Insights**
* **Key Drivers**
* **RM vs Agent**
* **Product Performance**
* **Policy Record View**

---

# 📘 Project Overview

This project simulates a **mini insurance analytics platform**.
It enables business users to analyze:

* Premium trends
* Customer ROI & profitability
* Policy maturity outcomes
* Agent and regional performance
* Product return performance
* Customer demographics
* Key drivers influencing premium and gain

The goal is to highlight:

* ✔️ SQL Data Warehousing
* ✔️ Dimensional Modeling
* ✔️ Business Logic Transformation
* ✔️ DAX + Power BI Storytelling
* ✔️ Real-World Insurance Metrics
* ✔️ Efficient ETL & Data Standardization

---

# 🏗️ Data Warehouse Architecture (Silver → Gold)

### ⭐ **Short Explanation (BI Knowledge Focused)**

This project adopts a **two-layer warehouse** (Silver → Gold) because the source CSV data was already clean and did not require a Bronze raw zone. The Silver layer standardizes and structures the data, while the Gold layer applies all insurance business rules, KPIs, and star-schema modeling to produce analytics-ready fact and dimension tables.
This approach keeps the solution efficient while demonstrating strong data warehousing principles.

---

## 🥈 **Silver Layer — Clean Staging**

The Silver layer stores clean, validated tables loaded directly from the data source.

### **Purpose**

* Apply schema consistency
* Preserve source meaning
* Validate data types
* Prepare data for transformation

### **Silver Tables**

* `silver.dim_customer`
* `silver.dim_agent`
* `silver.dim_policy_plan`
* `silver.dim_policy_type`
* `silver.dim_regional_manager`
* `silver.fact_insurance_policy`
* `silver.load_silver_insurance` *(automated loader)*

The ETL process:

* Bulk loads CSV files
* Clears old staging data
* Logs execution duration

---

## 🥇 **Gold Layer — Business Logic + Star Schema**

The Gold layer applies all rules required to calculate policy KPIs.

### ⭐ Key Business Logic in `gold.vw_insurance_policy_enriched`

* Annual premium standardization
* Premium paid vs payable
* Total tenure premium
* Maturity amounts
* Customer Profit & Gain
* Annualized ROI %
* Payment frequency buckets
* Policy tenure + remaining duration
* Maturity flags (5/10/15/20 years)

### ⭐ Gold Tables

* `gold.dim_customer`
* `gold.dim_sales_agent`
* `gold.dim_regional_manager`
* `gold.fact_insurance_policy` *(contains all enriched metrics)*
* `gold.load_gold` *(orchestration stored procedure)*

This layer forms a clean **star schema** optimized for Power BI.

---

# 📊 Power BI Analytics Workflow

Power BI connects directly to the Gold layer to generate an interactive insurance insights dashboard.

### Main Report Areas:

* **Customer Profitability**
* **Policy & Product Performance**
* **Regional & Agent Performance**
* **Premium Trends**
* **Maturity and ROI Insights**
* **Key Driver Analysis**
* **Demographics & Segmentation**

---

# ❓ Business Questions Answered

### **👤 Customer Profitability**

* Which customer segments generate the most profit?
* How much gain/ROI does each customer earn?
* Which payment frequency creates higher premiums?

### **📦 Policy & Product Insights**

* Which policy types generate the highest returns?
* How do tenure lengths affect maturity value?
* Which products deliver the strongest ROI?

### **📍 Regional & Agent Performance**

* Which regions/townships contribute the highest premium?
* Which RM/agents bring in the best customers?

### **📈 Premium & Trend Analytics**

* Monthly and yearly premium trends
* Underwriting expense variance
* Customer count growth over time

### **⏳ Operational Insights**

* Policies maturing in 5/10/15/20 years
* Amount paid vs remaining payable
* High-risk / low-return policies

---

# 🚀 Skills Demonstrated

* **SQL Data Warehousing (Silver/Gold)**
* **Dimensional & Star Schema Modeling**
* **Business Rules & KPI Design**
* **ETL Development (Stored Procedures, Bulk Insert)**
* **DAX & Power BI Visual Modeling**
* **Analytical Storytelling for Insurance Operations**

This project is built as a professional **BI/Analytics portfolio** piece to demonstrate real-world analytical engineering capabilities.

---

# ⭐ GitHub Stats (Auto-updates)

```md
![GitHub Repo Stars](https://img.shields.io/github/stars/PannPwintPhyu/Superstore-Analytics-Dashboard?style=for-the-badge)
![GitHub Forks](https://img.shields.io/github/forks/PannPwintPhyu/Superstore-Analytics-Dashboard?style=for-the-badge)
![GitHub Last Commit](https://img.shields.io/github/last-commit/PannPwintPhyu/Superstore-Analytics-Dashboard?style=for-the-badge)
![GitHub Issues](https://img.shields.io/github/issues/PannPwintPhyu/Superstore-Analytics-Dashboard?style=for-the-badge)
```
