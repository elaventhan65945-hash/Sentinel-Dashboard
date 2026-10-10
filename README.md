# ⚠️ SENTINEL
## Financial Risk Intelligence Dashboard
> *"Detecting Risk Before It Becomes Reality"*

---

## 📸 Dashboard Preview

### Page 1 — Risk Overview


![Page 1](Page1.png)



### Page 2 — Deep Dive Analysis


![Page 2](Page2.png)



---

## 📌 Project Overview
SENTINEL is a Power BI dashboard that analyzes 
loan default risk patterns to help banks identify 
high risk customers before approving loans.

---

## 📊 Dataset
- **Source:** Kaggle
- **Rows:** 20,000
- **Columns:** 23
- **Topic:** Financial Risk / Loan Default

---

## 🛠️ Tools Used
- Power BI Desktop
- Power Query (Data Cleaning)
- DAX (Data Analysis Expressions)
- Row Level Security (RLS)

---

## 🧹 Data Cleaning Steps
- Fixed null values in Credit Utilization 
  and Collateral Value
- Created group columns:
  - Age Group
  - Income Group
  - Credit Score Group
  - Loan Amount Group
- Extracted Year, Month, Quarter 
  from Loan Start Date
- Created Risk Categories using SWITCH function
- Converted Default Status (0/1) to 
  Defaulted/Paid

---

## 📐 Data Model
- Fact_Loans (Main Table)
- Dim_Customer
- Dim_Employment
- Dim_Date

---

## 📏 DAX Measures
| Measure | Function |
|---------|---------|
| Total Applications | COUNTROWS |
| Total Loan Amount | SUM |
| Avg Interest Rate | AVERAGE |
| Avg Credit Score | AVERAGE |
| Avg Credit Utilization | AVERAGE |
| Avg Debt to Income Ratio | AVERAGE |
| Total Collateral Value | SUM |
| High Risk Count | CALCULATE |
| Medium Risk Loans | CALCULATE |
| Low Risk Loans | CALCULATE |
| Rank by Age Group | RANKX |
| Avg Loan Term | AVERAGE |

---

## 🔐 Row Level Security (RLS)
| Role | Filter |
|------|--------|
| Urban Manager | Property_Area = Urban |
| Rural Manager | Property_Area = Rural |
| Semiurban Manager | Property_Area = Semiurban |

---

## 📄 Dashboard Pages

### Page 1 — Risk Overview
- 5 KPI Cards with Targets
- Line Chart — Loan & Interest Rate Trend
- Donut Chart — Loan Wise Risk
- Bar Chart — Employment Wise Risk
- Matrix Table — Age Group Risk (RANKX)
- Matrix Table — Credit Score Risk Distribution
- Gauge Chart — Existing Debt vs Collateral

### Page 2 — Deep Dive Analysis
- 5 KPI Cards with Targets
- Bar Chart — Payment Delay Analysis
- Bar Chart — Application by Credit Risk
- Waterfall Chart — Yearly Loan Growth
- Matrix Table — Quarterly Loan Performance
- Slicer — Employment Type Filter

---

## 🔍 Key Insights
- Middle Age (31-45) has highest loan default risk
- Salaried employees take highest loan amounts
- Poor credit score = Highest default risk
- Large loans have most defaults
- Higher payment delays = Higher default chance

---

## 📁 Project Structure
```
SENTINEL/
├── financial_risk_dataset.csv
├── SENTINEL.pbix
├── Page1.png
├── Page2.png
└── README.md
```

---

## 👤 Author
**Elaventhan**
Data Analyst | Power BI Developer
Chennai, Tamil Nadu

---
