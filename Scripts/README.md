# 📊 Intermediate SQL Project – Sales & Customer Analysis

## 📌 Project Overview
This project focuses on analyzing **customer behavior, retention, and lifetime value** for an e-commerce business using **SQL**.  
The objective is to extract **actionable business insights** that help improve customer retention, optimize revenue, and understand customer purchasing patterns.

---

## 🎯 Business Objectives
This analysis answers the following business questions:

1. **Customer Segmentation**  
   - Who are the most valuable customers?
   - How much revenue does each customer segment contribute?

2. **Cohort Analysis**  
   - How does revenue vary across different customer cohorts?
   - Are newer cohorts performing better or worse than older ones?

3. **Customer Retention Analysis**  
   - Which customers are at risk of churn?
   - When does churn typically occur?

---

## 🧹 Data Preparation & Cleanup

**SQL Script:** [create_view_main.sql](create_view_main.sql)

Key steps performed:
- Aggregated transactional data into customer-level revenue metrics  
- Identified each customer’s **first purchase date** for cohort analysis  
- Created a consolidated SQL **view** combining sales and customer details  
- Prepared clean, analysis-ready data for downstream queries  

---

## 📈 Analysis & Insights

---

### 1️⃣ Customer Segmentation

**SQL Script:** [1_customer_segmentation.sql](1_customer_segmentation.sql)

**Methodology:**
- Calculated **Customer Lifetime Value (LTV)**
- Segmented customers into **High, Mid, and Low-Value** groups
- Analyzed revenue contribution per segment

**Key Findings:**
- **High-Value Customers (25%)** generate **66% of total revenue (~$135.4M)**
- **Mid-Value Customers (50%)** generate **32% of total revenue (~$66.6M)**
- **Low-Value Customers (25%)** generate only **2% of revenue (~$4.3M)**

**Business Insights:**
- High-value customers are critical to revenue stability  
- Mid-value customers present strong **upsell opportunities**  
- Low-value customers require **cost-efficient re-engagement strategies**

---

### 2️⃣ Customer Revenue by Cohort

**SQL Script:** [2_cohort_analysis.sql](2_cohort_analysis.sql)

**Methodology:**
- Grouped customers by **year of first purchase**
- Tracked revenue and customer count by cohort
- Normalized revenue based on time in market
- Analyzed trends using rolling averages

**Key Findings:**
- Older cohorts (2016–2018) spent **~$2,800+ per customer**
- Newer cohorts (2024) spent **~$1,970**, showing declining spend
- Revenue and customer count peaked in **2022–2023**
- Noticeable drops in **2020 and 2024**, indicating retention challenges

**Business Insights:**
- Newer cohorts need stronger early engagement strategies  
- Revenue volatility suggests a need for **loyalty or subscription models**  
- Successful strategies from older cohorts can be applied to newer ones  

---

### 3️⃣ Customer Retention & Churn Analysis

**SQL Script:** [3_retention_analysis.sql](3_retention_analysis.sql)

**Methodology:**
- Identified customers at risk of churn using last purchase date
- Analyzed churn patterns across cohort years
- Studied long-term retention behavior

**Key Findings:**
- Churn stabilizes at **~90% after 2–3 years**
- Retention remains consistently low (**8–10%**) across all cohorts
- Newer cohorts follow similar churn patterns as older ones

**Business Insights:**
- The first **1–2 years** are crucial for customer retention  
- Retention issues are systemic, not cohort-specific  
- Targeted win-back campaigns for high-value churned customers offer higher ROI  

---

## 🧠 Strategic Recommendations

### Customer Value Optimization
- Launch a **VIP program** for high-value customers
- Create **personalized upgrade paths** for mid-value customers
- Use **price-sensitive promotions** for low-value customers

### Cohort Performance Strategy
- Focus re-engagement efforts on **2022–2024 cohorts**
- Introduce **loyalty or subscription-based programs**
- Replicate strategies from high-performing older cohorts

### Retention & Churn Prevention
- Strengthen onboarding and early engagement
- Run targeted win-back campaigns for valuable churned users
- Use proactive churn indicators for early intervention

---

## ⚙️ Technical Stack
- **Database:** PostgreSQL  
- **SQL Client:** DBeaver  
- **Analysis Language:** SQL  
- **Visualization:** Generated using ChatGPT  


