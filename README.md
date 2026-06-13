# Customer Churn Analysis & Retention Strategy

## Project Overview

Customer churn is one of the biggest challenges for subscription-based businesses, directly affecting recurring revenue and customer lifetime value (CLTV). This project analyzes customer behavior using the IBM Telco Customer Churn dataset to identify the key drivers of churn, quantify its business impact, and recommend data-driven retention strategies.

The project is being developed as an end-to-end analytics portfolio project using SQL, Python, and Tableau.

---

## Business Problem

A telecommunications company is experiencing customer churn and wants to answer several critical business questions:

* Which customers are most likely to churn?
* What factors contribute to customer churn?
* Which customer segments should be prioritized for retention?
* How much recurring revenue is lost due to churn?
* What actions can improve customer retention and reduce revenue loss?

---

## Project Objectives

* Analyze customer churn using SQL.
* Identify the primary drivers of customer churn.
* Segment customers based on contracts, services, tenure, and payment behavior.
* Measure the financial impact of customer churn.
* Provide actionable business recommendations backed by data.

---

## Dataset

**Dataset:** IBM Telco Customer Churn Dataset

The dataset contains information for **7,043 telecom customers**, including:

* Customer demographics
* Account information
* Contract details
* Internet services
* Billing and payment methods
* Monthly charges
* Customer churn status

---

## Tech Stack

| Tool                        | Purpose                                     | Status         |
| --------------------------- | ------------------------------------------- | -------------- |
| PostgreSQL                  | Business analysis using SQL                 | ✅ Completed    |
| Python (Pandas, Matplotlib) | Exploratory data analysis & visualization   | 🚧 In Progress |
| Tableau                     | Interactive dashboard & executive reporting | 🚧 In Progress |

---

# SQL Analysis (Completed)

The SQL phase answers **17 real-world business questions**, progressing from descriptive analysis to executive-level business insights.

### Phase 1 — Data Understanding

* Customer overview
* Overall churn metrics
* Contract distribution
* Contract-wise churn analysis

### Phase 2 — Customer Segmentation

* Internet service analysis
* Payment method analysis
* Customer tenure analysis
* Customer segment analysis

### Phase 3 — Retention Analysis

* Customer lifecycle analysis
* Online Security analysis
* Tech Support analysis
* Product add-on analysis

### Phase 4 — Business Impact Analysis

* Customer retention opportunity
* Monthly revenue loss estimation
* High-risk customer profile identification

---

# Key Business Findings

## Customer Overview

| Metric             |  Value |
| ------------------ | -----: |
| Total Customers    |  7,043 |
| Customers Churned  |  1,869 |
| Overall Churn Rate | 26.54% |

### 1. Contract Length Strongly Influences Customer Retention

| Contract       | Churn Rate |
| -------------- | ---------: |
| Month-to-month |     42.71% |
| One year       |     11.27% |
| Two year       |      2.83% |

**Insight**

Customers on Month-to-month contracts are nearly **15× more likely** to churn than customers on Two-year contracts.

---

### 2. Fiber Optic Customers Have the Highest Churn

| Internet Service    | Churn Rate |
| ------------------- | ---------: |
| Fiber optic         |     41.89% |
| DSL                 |     18.96% |
| No Internet Service |      7.40% |

**Insight**

Fiber Optic customers represent the highest-risk service segment and should be prioritized for retention initiatives.

---

### 3. Customer Churn Happens Early

Average customer tenure:

* **Retained customers:** 37.57 months
* **Churned customers:** 17.98 months

**Insight**

Most customer churn occurs during the first two years of the customer lifecycle.

---

### 4. Online Security and Tech Support Improve Retention

Customers who subscribe to **Online Security** and **Tech Support** experience significantly lower churn rates than customers who do not.

These two services demonstrate the strongest association with customer retention among all product add-ons analyzed.

---

### 5. Reducing Month-to-Month Churn Could Save Over 1,200 Customers

If Month-to-month customers experienced the same churn rate as One-year customers:

* **Customers retained:** **1,218**

This represents the largest opportunity for improving overall customer retention.

---

### 6. Customer Churn Results in Significant Revenue Loss

| Metric                                       |       Value |
| -------------------------------------------- | ----------: |
| Churned Customers                            |       1,869 |
| Estimated Monthly Revenue Lost               | $139,130.84 |
| Average Monthly Revenue per Churned Customer |      $74.44 |

**Insight**

Customer churn is responsible for approximately **$139K in recurring monthly revenue loss**, highlighting its direct financial impact.

---

### 7. Highest-Risk Customer Profile

Customers most likely to churn typically have the following characteristics:

* Month-to-month contract
* Fiber Optic internet service
* Less than two years of tenure
* No Tech Support
* Electronic Check payment method

This customer profile should be the primary target for future retention campaigns.

---

# Business Recommendations

Based on the analysis, the company should:

* Encourage customers to migrate from Month-to-month to longer-term contracts.
* Improve the onboarding experience for new customers during their first two years.
* Investigate the causes of high churn among Fiber Optic customers.
* Increase adoption of Online Security and Tech Support through bundled offerings.
* Prioritize proactive retention campaigns for customers matching the identified high-risk profile.

---

# Repository Structure

```text
customer-churn-analysis/
│
├── data/
│
├── sql/
│   ├── 01_customer_overview.sql
│   ├── 02_contract_analysis.sql
│   ├── 03_internet_service_analysis.sql
│   ├── 04_payment_method_analysis.sql
│   ├── 05_customer_segmentation.sql
│   ├── 06_tenure_analysis.sql
│   ├── 07_online_security_analysis.sql
│   ├── 08_tech_support_analysis.sql
│   ├── 09_product_addon_analysis.sql
│   ├── 10_retention_opportunity.sql
│   ├── 11_revenue_impact.sql
│   └── 12_high_risk_customer_profile.sql
│
├── findings.md
├── README.md
│
├── python/
│   └── (In Progress)
│
└── tableau/
    └── (In Progress)
```

---

# Current Project Status

| Component             | Status         |
| --------------------- | -------------- |
| SQL Business Analysis | ✅ Completed    |
| Business Findings     | ✅ Completed    |
| Python Analysis       | 🚧 In Progress |
| Tableau Dashboard     | 🚧 In Progress |

---

# Future Enhancements

* Exploratory Data Analysis (EDA) using Python
* Customer Lifetime Value (CLTV) analysis
* Geographic churn analysis
* Interactive Tableau dashboard
* Churn prediction using machine learning

---

## Author

**Sony Bachani**

Aspiring Data Scientist | Data Analyst

This project demonstrates how SQL can be used to solve real business problems by transforming raw customer data into actionable insights that support customer retention and revenue growth.
