# Customer Churn Analysis & Retention Strategy

## 📌 Project Overview

This project analyzes customer churn behavior for a telecom company using the IBM Telco Customer Churn dataset.

The objective is to identify **key drivers of churn, high-risk customer segments, and revenue impact**, and translate these insights into actionable retention strategies using SQL-based analysis.

---

## 🎯 Business Problem

The telecom company is facing high customer churn and wants to understand:

- Which customers are most likely to churn?
- What factors drive customer churn?
- Which customer segments are high-risk?
- What revenue impact does churn create?
- What retention strategies can reduce churn?

---

## 🧠 Project Objectives

- Analyze churn patterns using SQL
- Identify key churn drivers
- Segment customers by contract, tenure, services, and payment behavior
- Quantify churn impact using monthly charges
- Provide actionable retention recommendations

---

## 📊 Dataset

**IBM Telco Customer Churn Dataset**

- 7,043 customers
- Demographics, account details, services, billing, and churn status

---

## 🛠️ Tech Stack

| Tool       | Purpose |
|------------|--------|
| PostgreSQL | SQL-based business analysis |
| Python     | EDA & visualization (in progress) |
| Tableau    | Dashboard (in progress) |

---

## 🧮 SQL Analysis (Completed)

The analysis is structured into four logical phases:

### Phase 1: Customer Overview
- Overall churn metrics
- Customer distribution
- Contract structure analysis

### Phase 2: Customer Segmentation
- Internet service analysis
- Payment method analysis
- Tenure-based segmentation

### Phase 3: Retention Drivers
- Online Security impact
- Tech Support impact
- Add-on service analysis

### Phase 4: Business Impact Analysis
- Revenue impact of churn (based on MonthlyCharges)
- High-risk customer identification
- Contract conversion opportunity analysis

---

# 📈 Key Business Findings

## 1. Overall Customer Churn

| Metric | Value |
|--------|------:|
| Total Customers | 7,043 |
| Churned Customers | 1,869 |
| Churn Rate | 26.54% |

**Insight:**  
More than 1 in 4 customers have churned, indicating a significant retention challenge.

---

## 2. Contract Type is the Strongest Churn Driver

| Contract Type | Churn Rate |
|--------------|-----------:|
| Month-to-month | 42.71% |
| One Year | 11.27% |
| Two Year | 2.83% |

**Insight:**  
Month-to-month customers are significantly more likely to churn than long-term contract customers.

---

## 3. Fiber Optic Customers Have the Highest Churn

| Internet Service | Churn Rate |
|------------------|-----------:|
| Fiber optic | 41.89% |
| DSL | 18.96% |
| No Internet Service | 7.40% |

**Insight:**  
Fiber optic customers represent the highest-risk service segment.

---

## 4. Most Customers Churn Early in Their Lifecycle

| Tenure | Churn Rate |
|--------|-----------:|
| 0–1 Year | 47.44% |
| 1–2 Years | 28.71% |
| 2–3 Years | 21.63% |
| 3–4 Years | 19.03% |
| 4–5 Years | 14.42% |
| 5–6 Years | 6.61% |

**Insight:**  
Churn is heavily concentrated in the first 12 months of customer lifecycle.

---

## 5. Payment Method Influences Churn

| Payment Method | Churn Rate |
|----------------|-----------:|
| Electronic Check | 45.29% |
| Mailed Check | 19.11% |
| Bank Transfer (Auto) | 16.71% |
| Credit Card (Auto) | 15.24% |

**Insight:**  
Customers using Electronic Check are significantly more likely to churn.

---

## 6. Online Security Strongly Reduces Churn

| Online Security | Churn Rate |
|-----------------|-----------:|
| Yes | 14.61% |
| No | 41.77% |

**Insight:**  
Customers with Online Security are far more likely to be retained.

---

## 7. Tech Support Strongly Improves Retention

| Tech Support | Churn Rate |
|--------------|-----------:|
| Yes | 15.17% |
| No | 41.64% |

**Insight:**  
Tech Support adoption is strongly associated with lower churn.

---

## 8. Add-on Services with Highest Retention Impact

- Online Security → highest retention impact  
- Tech Support → high retention impact  
- Online Backup → moderate impact  
- Device Protection → moderate impact  
- Streaming Services → low impact  

**Insight:**  
Security and support services drive retention more than entertainment add-ons.

---

## 9. Revenue Impact of Churn (Based on Monthly Charges)

| Metric | Value |
|--------|------:|
| Churned Customers | 1,869 |
| Monthly Revenue Impact | $139,130 |
| Avg Monthly Charge (Churned) | $74.44 |

**Insight:**  
Churned customers represent significant monthly revenue contribution loss based on current billing amounts.

---

## 10. Contract Conversion Opportunity

If Month-to-month customers matched One-Year churn rates:

- Additional customers retained: **1,218**

**Insight:**  
Contract conversion represents the largest single retention opportunity.

---

## 11. High-Risk Customer Profile

Customers most likely to churn:

- Month-to-month contract
- Fiber optic internet
- Less than 1 year tenure
- No Tech Support
- Electronic Check payment

**Insight:**  
This segment shows churn rates exceeding 50% in some cases.

---

# 💡 Strategic Recommendations

- Focus retention efforts on Month-to-month customers in their first year
- Promote Online Security and Tech Support through bundling
- Encourage migration from Electronic Check to automatic payments
- Investigate Fiber optic customer experience issues
- Build a churn prediction model using identified risk factors
- Track churn and revenue impact using an executive dashboard

---

# 📁 Repository Structure

customer-churn-analysis/

├── data/
├── sql/                  # 17 SQL scripts
├── findings.md          # detailed breakdown
├── README.md
├── python/              # in progress
└── tableau/             # in progress

---

# 🚧 Project Status

| Component | Status |
|----------|--------|
| SQL Analysis | ✅ Completed |
| Business Findings | ✅ Completed |
| Python EDA | 🚧 In Progress |
| Tableau Dashboard | 🚧 In Progress |

---

## 👤 Author

**Sony Bachani**  
Aspiring Data Scientist | Data Analyst

---

## 📌 Summary

This project demonstrates how SQL can be used to transform raw customer data into **actionable business insights that support retention strategy and revenue protection**, without relying on predictive modeling.
