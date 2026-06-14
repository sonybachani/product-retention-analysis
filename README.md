# Customer Churn Analysis & Retention Strategy

## 📌 Project Overview

This project analyzes customer churn behavior for a telecom company using the IBM Telco Customer Churn dataset.

The goal is to identify **key drivers of churn, high-risk customer segments, and revenue impact**, and translate these insights into actionable retention strategies using SQL-based analysis.

---

## 🎯 Business Problem

The company is facing high customer churn and wants to understand:

- Which customers are most likely to churn?
- What factors drive customer churn?
- Which customer segments are high-risk?
- What is the financial impact of churn?
- What retention strategies can reduce churn?

---

## 📊 Dataset

**IBM Telco Customer Churn Dataset**

- 7,043 customers
- Includes demographics, account details, services, billing, and churn status

---

## 🛠️ Tech Stack

| Tool       | Purpose |
|------------|--------|
| PostgreSQL | SQL-based business analysis |
| Python     | EDA & visualization (in progress) |
| Tableau    | Dashboard (in progress) |

---

## 🧮 Analysis Approach

The analysis is structured into four areas:

1. Customer Overview & Churn Measurement  
2. Customer Segmentation (contract, tenure, payment, services)  
3. Churn Driver Analysis (security, tech support, add-ons)  
4. Business Impact (revenue + high-risk profiling)

---

# 📈 Key Insights

## 1. Overall Churn Rate
- Total Customers: **7,043**
- Churned Customers: **1,869**
- Churn Rate: **26.54%**

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

## 3. Fiber Optic Customers Are High Risk

| Internet Service | Churn Rate |
|------------------|-----------:|
| Fiber optic | 41.89% |
| DSL | 18.96% |
| No Internet | 7.40% |

**Insight:**  
Fiber optic customers represent the highest-risk service segment.

---

## 4. Churn is Highest in Early Tenure

| Tenure | Churn Rate |
|--------|-----------:|
| 0–1 Year | 47.44% |
| 1–2 Years | 28.71% |
| 2–3 Years | 21.63% |
| 3–4 Years | 19.03% |
| 4–5 Years | 14.42% |
| 5–6 Years | 6.61% |

**Insight:**  
The first year of customer lifecycle is the most critical churn period.

---

## 5. Key Services Improve Retention

Customers with:
- Online Security
- Tech Support

show significantly lower churn rates.

**Insight:**  
Support and security services strongly improve customer retention.

---

## 6. Revenue Impact of Churn

- Churned Customers: **1,869**
- Monthly Revenue Impact: **$139,130**
- Avg Monthly Charge (Churned): **$74.44**

**Insight:**  
Churned customers represent significant monthly revenue contribution loss based on current billing.

---

## 7. High-Risk Customer Profile

Customers most likely to churn:

- Month-to-month contract
- Fiber optic internet
- Less than 1 year tenure
- No Tech Support
- Electronic Check payment method

**Insight:**  
This segment shows churn rates exceeding 50% in some cases.

---

## 💡 Business Recommendations

- Focus retention efforts on Month-to-month customers in their first year
- Promote Online Security and Tech Support through bundling
- Encourage migration from Electronic Check to automatic payments
- Investigate Fiber optic customer experience issues
- Build a churn prediction model using identified risk factors
- Monitor churn and revenue impact using dashboards

---

## 📁 Repository Structure
customer-churn-analysis/

├── data/
│
├── sql/                  # 17 SQL scripts
│
├── findings.md          # detailed analysis
│
├── README.md
│
├── python/              # in progress
│
└── tableau/             # in progress

---

## 🚧 Project Status

| Component | Status |
|----------|--------|
| SQL Analysis | ✅ Completed |
| Business Insights | ✅ Completed |
| Python EDA | 🚧 In Progress |
| Tableau Dashboard | 🚧 In Progress |

---

## 👤 Author

**Sony Bachani**  
Aspiring Data Scientist | Data Analyst

---

## 📌 Summary

This project demonstrates how SQL can be used to transform raw customer data into **actionable business insights that support retention strategy and revenue impact analysis**.
