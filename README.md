# FUTURE_DS_02

#  SaaS Customer Churn Analysis using Power BI

##  Project Overview
Customer churn is a critical challenge for SaaS and subscription-based businesses. This project focuses on analyzing customer, subscription, engagement, support, and churn data to understand **why customers leave**, **which segments are most at risk**, and **what actions can improve retention**.

The analysis mirrors real-world work performed by data analysts in **product, growth, and retention teams**, using Power BI to convert raw data into actionable business insights.

---

##  Objectives
- Measure customer churn and retention performance
- Identify customer segments with higher churn risk
- Analyze product engagement and support experience
- Understand key churn reasons
- Provide data-driven recommendations to improve customer retention

---

##  Dataset Description
The project uses multiple interconnected datasets:

- **ravenstack_accounts**  
  Customer master data including plan tier, churn flag, country, industry, and signup date.

- **ravenstack_subscriptions**  
  Subscription lifecycle details such as start date, end date, and plan information.

- **ravenstack_feature_usage**  
  Product engagement data capturing feature usage counts and activity duration.

- **ravenstack_support_tickets**  
  Customer support interactions including ticket count and resolution time.

- **ravenstack_churn_events**  
  Churn events with churn dates, reason codes, and customer feedback.

---

##  Tools & Technologies
- **Power BI Desktop**
- **Power Query** (data cleaning & transformation)
- **DAX (Data Analysis Expressions)**
- **Data Modeling (Star Schema)**

---

##  Data Preparation & Modeling
1. Imported all datasets into Power BI using Power Query  
2. Cleaned and transformed data by:
   - Correcting data types
   - Removing duplicate records
   - Handling missing and blank values  
3. Built a **star schema** data model with:
   - `ravenstack_accounts` as the central dimension table
   - Fact tables for subscriptions, feature usage, support tickets, and churn events  
4. Created relationships using `account_id` as the primary key

---

##  Key Metrics & KPIs
The following KPIs were created using DAX:

- **Total Customers**
- **Active Customers**
- **Churned Customers**
- **Churn Rate (%)**
- **Average Customer Lifetime (Days)**

These KPIs provide a high-level overview of churn and retention performance.

---

##  Analysis Performed

### 1️⃣ Churn by Subscription Plan
- Compared churned customers across plan tiers
- Identified higher churn in lower-tier plans

### 2️⃣ Product Engagement vs Churn
- Compared feature usage between active and churned customers
- Observed that **low product engagement strongly correlates with churn**

### 3️⃣ Support Experience Impact on Churn
- Analyzed total support tickets raised by active vs churned customers
- Found that frequent support interactions are associated with higher churn risk

### 4️⃣ Churn Reasons Analysis
- Used churn event data to analyze churn by `reason_code`
- Identified top churn drivers such as:
  - Pricing and budget constraints
  - Feature limitations
  - Support issues
  - Competitive alternatives

### 5️⃣ Customer Lifetime & Retention Analysis
- Measured average customer lifetime
- Analyzed customer behavior patterns over time

---

##  Dashboard Design
A single-page Power BI dashboard was designed with:
- **Top KPI cards** for executive-level insights
- **Churn driver visuals** (plan tier, engagement, support)
- **Churn reason analysis** for root-cause identification

The dashboard follows a clean and structured layout suitable for business stakeholders.

---

##  Key Insights
- Overall churn rate is **22%**, indicating a significant retention opportunity
- Lower-tier plans experience higher churn
- Customers with low feature usage are more likely to churn
- Support experience plays a key role in churn behavior
- Pricing and feature gaps are the most common churn reasons

---

##  Business Recommendations
- Improve onboarding and feature adoption for new users
- Proactively engage low-usage customers
- Enhance support response and resolution times
- Revisit pricing and plan value propositions
- Improve churn feedback collection to reduce unknown churn reasons

---

##  Conclusion
This project demonstrates an end-to-end **SaaS churn analysis workflow**, covering data preparation, modeling, KPI creation, behavioral analysis, and business recommendations. It reflects real-world analytics practices and showcases practical Power BI and DAX skills.

---

##  Author
**Mohan Kumar**  
Data Analytics | Power BI | SaaS Analytics
