# 🚀 Welcome to the **Insurance Business Insights** project   


This project showcases my practical BI skillset across data modeling, ETL design, business logic implementation, and storytelling using an optimized analytical data warehouse.

---

## 🔗 Live Power BI Dashboard

 **View Interactive Report**
https://app.powerbi.com/view?r=eyJrIjoiMDI2YjQzZDgtODkwYi00YTM3LTg1YmItZDc0ZjdmZDQ0Njk1IiwidCI6IjhlZjRhZjJkLTkwY2YtNGIzMS1hMTI4LTNmYWE5M2EzMmJjOCIsImMiOjEwfQ%3D%3D

---

##  Dashboard Preview

<table> <tr> <td><img src="https://github.com/PannPwintPhyu/insurance_business_insights_report/blob/main/assets/1_Dashboard.png" alt="Dashboard" /></td> <td><img src="https://github.com/PannPwintPhyu/insurance_business_insights_report/blob/main/assets/2_Performance_Metrics.png" alt="Performance Metrics" /></td> <td><img src="https://github.com/PannPwintPhyu/insurance_business_insights_report/blob/main/assets/3_Customer_Insights.png" alt="Customer Insights" /></td> </tr> <tr> <td><strong>Main Dashboard</strong></td> <td><strong>Performance Metrics</strong></td> <td><strong>Customer Insights</strong></td> </tr> <tr> <td><img src="https://github.com/PannPwintPhyu/insurance_business_insights_report/blob/main/assets/4_RM_vs_Agent.png" alt="RM vs Agent" /></td> <td><img src="https://github.com/PannPwintPhyu/insurance_business_insights_report/blob/main/assets/5_KeyDrivers.png" alt="Key Drivers" /></td> <td><img src="https://github.com/PannPwintPhyu/insurance_business_insights_report/blob/main/assets/6_Record.png" alt="Record View" /></td> </tr> <tr> <td><strong>RM vs Agent</strong></td> <td><strong>Key Drivers</strong></td> <td><strong>Record View</strong></td> </tr> </table>

* **Main Dashboard**
* **Product Performance**                                                                
* **Customer Insights**                                                                              
* **RM vs Agent**                                                                                              
* **Key Drivers**
* **Policy Record View**

---

#  Project Overview

This project simulates a **mini insurance analytics platform**.
It enables business users to analyze:

* Premium trends
* Customer ROI & profitability
* Policy maturity outcomes
* Agent and regional performance
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

#  Data Warehouse Architecture (Silver → Gold)

This project adopts a **two-layer warehouse** (Silver → Gold) because the source CSV data was already clean and did not require a Bronze raw zone. The Silver layer standardizes and structures the data, while the Gold layer applies all insurance business rules, KPIs, and star-schema modeling to produce analytics-ready fact and dimension tables.
This approach keeps the solution efficient while demonstrating strong data warehousing principles.

---

##  **Silver Layer _ Clean Staging**

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
* `silver.load_silver_insurance` (orchestration stored procedure)

The ETL process:

* Bulk loads CSV files
* Clears old staging data
* Logs execution duration

---

##  **Gold Layer _ Business Logic + Star Schema**

The Gold layer applies all rules required to calculate policy KPIs.

###  Key Business Logic in `gold.vw_insurance_policy_enriched`

* Annual premium standardization
* Premium paid vs payable
* Total tenure premium
* Maturity amounts
* Customer Profit & Gain
* Annualized ROI %
* Payment frequency buckets
* Policy tenure + remaining duration
* Maturity flags (5/10/15/20 years)

###  Gold Tables

* `gold.dim_customer`
* `gold.dim_sales_agent`
* `gold.dim_regional_manager`
* `gold.fact_insurance_policy` *(contains all enriched metrics)*
* `gold.load_gold` *(orchestration stored procedure)*

This layer forms a clean **star schema** optimized for Power BI.

---

#  Power BI Analytics Workflow

Power BI consumes the Gold layer fact and dimension tables in Import Mode, enabling high-performance analytics on top of a star-schema model.

### Main Report Areas:

* **Customer Profitability**
* **Policy & Product Performance**
* **Regional & Agent Performance**
* **Premium Trends**
* **Maturity and ROI Insights**
* **Key Driver Analysis**
* **Demographics & Segmentation**

---

# ❓ Business Questions Answerer

###  Customer Profitability

* Which customer segments generate the most profit?
* How much gain/ROI does each customer earn?
* Which payment frequency creates higher premiums?

###  Policy & Product Insights

* Which policy types generate the highest returns?
* How do tenure lengths affect maturity value?
* Which products deliver the strongest ROI?

###  Regional & Agent Performance

* Which regions/townships contribute the highest premium?
* Which RM/agents bring in the best customers?

###  Premium & Trend Analytics

* Monthly and yearly premium trends
* Underwriting expense variance
* Customer count growth over time

###  Operational Insights

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


