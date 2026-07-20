# 🏦 Bank Loan Analytics Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-Analysis-blue)
![DAX](https://img.shields.io/badge/DAX-Measures-orange)
![Status](https://img.shields.io/badge/Project-Completed-success)

## 📖 Overview

The **Bank Loan Analytics Dashboard** is an end-to-end Business Intelligence project designed to analyze loan portfolio performance, borrower behavior, repayment trends, and credit risk. Using **SQL, Power BI, and DAX**, the dashboard transforms raw lending data into actionable insights that support better lending decisions and portfolio management.

The solution provides stakeholders with a comprehensive view of loan applications, funded amounts, repayment performance, borrower demographics, risk exposure, and strategic recommendations.

---

## 🎯 Business Problem

Financial institutions process thousands of loan applications across multiple borrower segments and regions. Without centralized reporting, it becomes difficult to:

- Monitor portfolio performance.
- Track repayment trends.
- Identify high-risk borrowers.
- Understand customer behavior.
- Optimize lending strategies.

This dashboard addresses these challenges through interactive analytics and executive-level reporting.

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|--------|
| Power BI | Dashboard Development |
| SQL | Data Extraction & Analysis |
| DAX | KPI & Business Logic |
| Power Query | Data Transformation |
| Excel / CSV | Source Dataset |

---

# 📊 Dashboard Pages

---

## 1️⃣ Executive Overview

### Purpose
Provides a high-level snapshot of overall portfolio performance.

### KPIs
- Loan Applications
- Total Funded Amount
- Total Amount Received
- Good Loan %
- Bad Loan %
- Average Interest Rate
- Average Credit Score
- Default Rate
- Recovery Rate
- Outstanding Amount

### Visuals
- Monthly Loan Application Trend
- Loan Status Distribution
- State-wise Funded Amount Map
- Loan Purpose Analysis

### Key Business Question
> How is the overall loan portfolio performing?

---

## 2️⃣ Loan Performance Analysis

### Purpose
Evaluates lending efficiency and repayment performance.

### KPIs
- Paid Loans
- Default Loans
- Current Loans
- Recovery Rate
- Default Rate
- Average Interest Rate

### Visuals
- Grade Performance Analysis
- Funded vs Received Amount
- Recovery Rate Gauge
- Loan Status Trend

### Key Business Question
> Which loan segments are generating the best returns?

---

## 3️⃣ Risk Analytics

### Purpose
Identifies high-risk borrower segments and default patterns.

### KPIs
- Average DTI
- High Risk Loans
- Average Credit Score
- Default Rate
- High Risk Exposure
- Bad Loan %

### Visuals
- Default Rate by Credit Score
- Loan Applications by Customer Segment
- Default Rate by Income Band
- High-Risk Borrower Table

### Key Business Question
> What factors contribute most to loan defaults?

---

## 4️⃣ Customer Analytics

### Purpose
Analyzes borrower demographics and lending behavior.

### KPIs
- Total Customers
- Average Income
- Average Loan Amount
- Average Credit Score
- Total States

### Visuals
- Income vs Loan Amount
- Employment Analysis
- Customer Segment Performance
- Home Ownership Distribution

### Key Business Question
> Who are the borrowers and how do they behave?

---

## 5️⃣ Executive Insights & Recommendations

### Insights

📌 Good loans represent the majority of the portfolio, indicating healthy lending performance.

📌 Borrowers with lower credit scores and higher DTI ratios contribute significantly to defaults.

📌 Debt Consolidation and Credit Card loans account for the largest share of funded amounts.

📌 Experienced borrowers demonstrate stronger repayment behavior compared to new borrowers.

📌 Portfolio concentration exists across a limited number of states and loan purposes.

### Recommendations

✅ Focus lending efforts on borrowers with strong credit profiles.

✅ Strengthen underwriting policies for high-risk segments.

✅ Implement proactive monitoring for borrowers with elevated DTI ratios.

✅ Diversify lending exposure across regions and loan purposes.

✅ Increase lending in high-performing borrower segments.

✅ Regularly review risk thresholds and credit policies.

✅ Develop retention programs for reliable borrowers.

✅ Utilize predictive risk scoring for early default detection.

---

# 📈 Key Metrics Calculated

| Metric | Formula |
|----------|----------|
| Good Loan % | Good Loans / Total Applications |
| Bad Loan % | Charged-Off Loans / Total Applications |
| Recovery Rate | Amount Received / Funded Amount |
| Default Rate | Default Loans / Total Applications |
| Avg Interest Rate | Average Interest Rate |
| Avg Credit Score | Average Credit Score |
| Outstanding Amount | Funded Amount - Amount Received |

---

# 🧮 Sample DAX Measures

### Total Applications

```DAX
Total Applications =
COUNT(bank_loan[id])
```

### Total Funded Amount

```DAX
Total Funded Amount =
SUM(bank_loan[loan_amnt])
```

### Total Amount Received

```DAX
Total Amount Received =
SUM(bank_loan[total_pymnt])
```

### Default Rate

```DAX
Default Rate =
DIVIDE(
    [Default Loans],
    [Total Applications]
)
```

### Recovery Rate

```DAX
Recovery Rate =
DIVIDE(
    [Total Amount Received],
    [Total Funded Amount]
)
```

---

# 🔍 Key Findings

- Over **147K loan applications** were analyzed.
- Total funded amount exceeded **$2.2 Billion**.
- Portfolio maintains a strong proportion of performing loans.
- Credit score and DTI are primary indicators of default risk.
- Experienced borrowers show better repayment behavior.
- Home ownership status impacts borrowing patterns.
- Geographic lending performance varies significantly across states.

---

# 🚀 Business Impact

This dashboard enables stakeholders to:

- Monitor portfolio health in real time.
- Identify high-risk borrower segments.
- Improve lending decisions.
- Reduce default exposure.
- Optimize portfolio allocation.
- Support data-driven financial strategies.

---

## 📸 Dashboard Preview

### Cover Page
![Cover Page](images/capture3.png)

### Overview
![Overview](images/Capture33.png)

### Loan Performance
![Loan Performance](images/Capture333.png)

### Risk Analytics
![Risk Analysis](images/Capture3333.png)

### Customer Analytics
![Customer Analysis](images/Capture33333.png)

### Insights & Recommendations
![Insights & Recommnedations](images/Capture333333.png)

---

## 👨‍💻 Author

**Vrind Mangla**

Data Analytics | Business Intelligence | Power BI | SQL

📧 Connect with me on LinkedIn for feedback and collaboration.

---

⭐ If you found this project useful, don't forget to star the repository.
