# Telecom Customer Churn & Retention Analysis

## 1. Background and Overview
**Objective:**
Customer churn, the loss of customers over time, is a critical challenge for telecom companies. High churn leads to revenue loss and increased costs of acquiring new customers. This project analyzes **7,043 telecom customers** to identify patterns in churn behavior, understand the factors driving churn, and provide actionable retention strategies.

**Scope:**
* **Focus:** Visual analysis and insights (no predictive modeling).
* **Goal:** Use demographic, service, and billing information to identify high-risk customer segments.
* **Tools:** Dashboard designed for executive decision-making with KPIs, filters, and interactive visuals.

---

## 2. Data Structure Overview
The analysis uses a dataset with **21 columns and 7,043 records**. The data is clean with no missing churn labels.

| Category | Columns | Purpose |
| :--- | :--- | :--- |
| **Customer Demographics** | `Gender`, `SeniorCitizen`, `Partner`, `Dependents` | Understand customer background and potential churn trends. |
| **Service & Subscription** | `Contract`, `PhoneService`, `InternetService`, `Streaming TV` | Identify churn risk based on service adoption. |
| **Billing & Usage** | `MonthlyCharges`, `TotalCharges`, `PaperlessBilling`, `PaymentMethod` | Analyze spending patterns and their impact on churn. |
| **Tenure** | `Tenure` | Measure customer loyalty and early churn risk. |
| **Churn Outcome** | `Churn` (Yes/No) | Key metric for retention analysis. |

---

## 3. Executive Summary
### Key Metrics
* **Total Customers:** 7,043
* **Churn Rate:** 26.54% (~1 in 4 customers)
* **Average Monthly Bill:** $64.76
* **Average Tenure:** 32.37 months

### Top-Level Diagnosis
The analysis indicates a moderate churn challenge where **short-tenure customers (<12 months)** have the highest churn rates. Customers with **high monthly charges** combined with short tenure show increased churn risk, and those on **Month-to-month contracts** are the most vulnerable segment.

---

## 4. Insights Deep Dive

### A. The "Year 1" Critical Zone
* **Observation:** Churn is highest in the first 12 months.
* **Implication:** The histogram shows early churn concentrated in the 0-12 month range; customers with longer tenure are much less likely to churn.

### B. Charges vs. Tenure Risk
* **Observation:** Scatter plot analysis shows that customers with **high monthly charges** and **short tenure** have the highest churn risk.
* **Opportunity:** Introduce discounts or loyalty incentives for high-charge new customers to reduce "sticker shock".

### C. Contract & Service Trends
* **Contract:** Month-to-month contract customers have significantly higher churn than those on 1- or 2-year contracts.
* **Service:** Fiber optic users are slightly more likely to churn than DSL or no-internet users.
* **Payment:** Methods like "Electronic check" see higher churn, indicating potential billing friction.

---

## 5. Recommendations

Based on the visualization data, the following strategic actions are recommended:

1.  **Retention Programs for New Customers:** Target customers in their first year with loyalty programs and proactive support to bridge the "Year 1" gap.
2.  **Contract Incentives:** Encourage month-to-month customers to switch to 1- or 2-year contracts through discounts or added benefits.
3.  **Billing & Service Optimization:** Monitor high monthly charges and consider flexible payment plans. Focus on electronic check users for payment reminders or automated support.
4.  **Customer Segmentation for Marketing:** Prioritize high-risk segments (short tenure, high charges, month-to-month contracts) for personalized campaigns.
5.  **Continuous Dashboard Monitoring:** Use the interactive dashboard to track churn trends in real-time and measure the impact of retention strategies.
