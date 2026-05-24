# Automated A/B Testing Pipeline: Python (Google Colab) to Tableau BI

An end-to-end analytical pipeline that automates A/B test interpretation for product management. The project bridges statistical computing in Python with interactive business intelligence in Tableau, transforming raw experimental data into automated, data-driven decisions.

## 📊 Dashboard Preview
[*The dashboard acts as an automated business interpreter](https://public.tableau.com/views/AB_17786003379130/Significance?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
. Stakeholders select a `Test Number` to view an instant text and visual summary of experimental performance, translating statistical confidence into clear corporate actions.*

---

## 🚀 Project Overview & Business Value
Manually evaluating A/B tests across multiple product metrics introduces human error and operational bottlenecks. This project solves that constraint by:
1. **Automating Statistical Computations:** Eliminating manual calculation of standard errors, Z-scores, and p-values.
2. **Standardizing Visual Insights:** Color-coding metrics inside Tableau based strictly on mathematical thresholds (statistical significance vs. random noise).
3. **Enhancing Stakeholder Autonomy:** Empowering product managers to self-serve A/B test results without querying data analysts.

---

## 🛠️ Tech Stack & Methodology
* **Data Processing & Scripting:** Python (`Pandas`, `NumPy`)
* **Statistical Engine:** `SciPy Stats` (Two-Sample Proportion Z-Test)
* **Environment:** Google Colab integrated with Google Drive cloud storage
* **Business Intelligence:** Tableau Desktop / Public (Advanced layout hierarchy & conditional formatting)

### Mathematical Framework
The core pipeline evaluates two-tailed hypothesis testing at a **95% confidence level ($\alpha = 0.05$)**:
* **Null Hypothesis ($H_0$):** $CR_{control} = CR_{test}$ (No actual difference in conversion rates).
* **Alternative Hypothesis ($H_1$):** $CR_{control} \neq CR_{test}$ (The product change caused a statistically significant shift).

---
