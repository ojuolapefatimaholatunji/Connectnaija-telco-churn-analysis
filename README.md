# ConnectNaija Telco — Customer Churn Analysis
### Built with Microsoft Power BI

---

## 📌 Project Overview

This project analyses customer churn for **ConnectNaija Telco** — 
a fictional telecommunications company serving 7,043 customers. 
Despite generating consistent revenue the company is losing 
**1 in every 4 customers** with no structured visibility into 
why customers are leaving or which segments are most at risk.

This two-page interactive Power BI dashboard identifies the 
drivers of churn and provides the retention team with clear, 
actionable recommendations to reduce the 26.5% churn rate.

---

## ❓ Business Problem

> *"ConnectNaija Telco is experiencing a 26.5% churn rate — 
> meaning 1,869 of its 7,043 customers have left. The company 
> has no visibility into which customers are most likely to 
> leave, what factors are driving their decision and which 
> segments require urgent intervention. Management needs a 
> financial performance analyst to profile the churning customer, 
> identify the highest risk segments and provide clear 
> recommendations that the retention team can implement 
> immediately to reduce churn before it further erodes revenue."*

---

## 📊 Dashboard Preview

### Page 1 — Churn Overview
![Overview Dashboard](assets/Page%201.png)

### Page 2 — Churn Driver Analysis
![Drivers Dashboard](assets/Page%202.png)

---

## 🔍 Insight Questions

**Page 1 — Overview:**
1. What is the overall scale of the churn problem?
2. Which contract type has the highest churn rate?
3. How does churn rate vary across customer tenure groups?
4. Which internet service type has the highest churn?

**Page 2 — Driver Analysis:**

5. Which payment method is most associated with churn?

6. Do value-added services (Tech Support, Online Security) reduce churn?
   
7. Are senior citizens more likely to churn than non-seniors?
   
8. What does the complete profile of a churning customer look like?

---

## 💡 Key Findings

**Finding 1 — 1 in 4 customers is leaving**

ConnectNaija has a 26.54% churn rate — 1,869 customers 
lost out of 7,043. Churned customers pay an average of 
$74.44/month compared to $61.27 for retained customers, 
meaning the company is losing its highest-paying customers first.

**Finding 2 — Month-to-month contracts are a churn machine**

Customers on month-to-month contracts churn at 42.71% — 
15x higher than two-year contract customers at 2.83%. 
This single factor is the most powerful predictor of churn 
in the entire dataset.

**Finding 3 — The first 12 months are the danger zone**

Customers in their first 0-12 months churn at 47.44% — 
nearly double the overall average. After 5 years the 
churn rate drops to just 6.61%. The company has a 
critical 12-month window to build loyalty.

**Finding 4 — Fiber optic customers churn the most**

Despite being the premium service Fiber optic customers 
churn at 41.89% — more than double DSL customers at 18.96%. 
This suggests a pricing or service quality problem with 
the Fiber product.

**Finding 5 — Electronic check is the highest risk payment method**

Electronic check customers churn at 45.29% — 3x higher 
than credit card (automatic) customers at 15.24%. Manual 
payment customers show significantly lower commitment levels.

**Finding 6 — Add-on services dramatically reduce churn**

Customers without Online Security churn at 41.77% vs 
14.61% with it — a 27.16% difference. Customers without 
Tech Support churn at 41.64% vs 15.17% with it. 
These services are retention tools not just revenue generators.

**Finding 7 — Senior citizens are the most vulnerable segment**

Senior citizens churn at 41.68% — nearly double the 
23.61% rate of non-senior customers. This segment 
requires a dedicated retention programme.

---

## 👤 The Churning Customer Profile

| Attribute | Profile |
|---|---|
| Contract | Month-to-month |
| Payment | Electronic check |
| Internet | Fiber optic |
| Security | No Online Security |
| Tech Support | No Tech Support |
| Tenure | 0–12 Months |
| Segment | Senior Citizen |
| Avg Monthly Charge | $74.44 |

---

## ✅ Recommendations

**Recommendation 1 — Incentivise contract upgrades**

Offer month-to-month customers a 10-15% discount to 
switch to annual contracts. Converting even 20% of 
month-to-month customers would reduce overall churn 
by approximately 8 percentage points.

**Recommendation 2 — Intervene in the first 12 months**

Create a dedicated onboarding programme for new customers 
— proactive check-ins, welcome offers and usage guidance 
during the critical first year when churn risk is highest.

**Recommendation 3 — Investigate Fiber optic service quality**

With a 41.89% churn rate on the premium product something 
is wrong. Commission a customer satisfaction survey 
specifically for Fiber optic users to identify pricing, 
speed or reliability issues before more customers leave.

**Recommendation 4 — Move customers to automatic payment**

Offer a small monthly discount (1-2%) to customers who 
switch from electronic check to automatic payment methods. 
This simple change could significantly reduce churn in 
the highest-risk payment segment.

**Recommendation 5 — Bundle add-on services for new customers**

Include Tech Support and Online Security in new customer 
onboarding packages at a reduced rate. Customers who adopt 
these services churn at less than half the rate of those 
without them — making them the most cost-effective 
retention tool available.

**Recommendation 6 — Launch a Senior Citizen retention programme**

Design specific retention offers for customers aged 65+ — 
simplified billing, dedicated support lines and loyalty 
discounts. At 41.68% churn this segment represents an 
immediate and addressable retention opportunity.

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Microsoft Power BI | Dashboard design and visualisation |
| Power Query | Data cleaning and transformation |
| DAX | Calculated measures and dynamic insights |
| IBM Telco Dataset | Source data |

---

---

## 📂 Dataset Information

| Field | Detail |
|---|---|
| Source | IBM Sample Dataset (Kaggle) |
| Records | 7,043 customers |
| Features | 21 columns |
| Target Variable | Churn (Yes/No) |
| Key Variables | Contract, Payment Method, Internet Service, Tenure, Add-on Services |

---

## 🔧 Data Cleaning Steps

1. Converted TotalCharges from text to decimal number
2. Replaced 11 blank TotalCharges values with 0
   (new customers with zero tenure)
3. Converted SeniorCitizen from 0/1 to Yes/No labels
4. Created Tenure Group calculated column
   (0-12, 13-24, 25-36, 37-48, 49-60, 61-72 months)
5. Unpivoted add-on service columns for clustered 
   bar chart comparison

---

## 📐 DAX Measures Written

- Churn Rate
- Retention Rate
- Churned Customers
- Retained Customers
- Avg Monthly Charges (Churned vs Retained)
- Avg Tenure (Churned)
- Dynamic churning customer profile card
- YoY measures for all KPIs
- Conditional color measures for YoY indicators
- Service churn rate (from unpivoted table)

---

## 👤 About the Analyst

**Fatimah Olatunji**
Data Analyst | Business Administration Graduate
Obafemi Awolowo University (OAU)


[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat&logo=linkedin)](www.linkedin.com/in/fatimah-olatunji-7665b73b6)
[![Twitter](https://img.shields.io/badge/Twitter-Follow-1DA1F2?style=flat&logo=twitter)](https://twitter.com/ojuolape124)

---

*This project was built as part of my ongoing data analytics 
learning journey. Every step — from data cleaning to DAX 
measures to dashboard design — was documented publicly 
on LinkedIn, Twitter and TikTok.*
