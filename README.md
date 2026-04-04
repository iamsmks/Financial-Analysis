# 📊 Financial Dashboard (Power BI)

## 🚀 Overview
This project presents an interactive **Financial Dashboard** built using Power BI to analyze a company's financial performance.  
It provides insights into **revenue, profitability, cash flow, and budget performance** with dynamic filtering and drill-down capabilities.

---

## 🎯 Objectives
- Monitor key financial KPIs  
- Compare **Budget vs Actual performance**  
- Analyze **cash flow and liquidity**  
- Evaluate performance across **regions and products**  
- Enable **interactive decision-making**

---

## 📂 Dataset
The dataset includes:

### Profit & Loss
- Revenue  
- COGS  
- Gross Profit  
- Operating Expenses (Opex)  
- EBITDA  

### Cash Flow
- Cash Inflows  
- Cash Outflows  

### Sales Information
- Product/Service  
- Region  
- Month  

### Aging Metrics
- Receivables Aging (Days)  
- Payables Aging (Days)  

### Budget Data
- Revenue Budget  
- Budget Variance %  

---

## 🧹 Data Preparation
- Cleaned and validated dataset (no missing values)  
- Ensured proper data types (Date, Numeric)  
- Created a **Date Table** for time-based analysis  
- Built relationships for efficient data modeling  

---

## 📐 Key Metrics (DAX)

```DAX
Total Revenue = SUM(Financial[Revenue])

Gross Margin % = 
DIVIDE(SUM(Financial[Gross Profit]), SUM(Financial[Revenue]))

EBITDA % = 
DIVIDE(SUM(Financial[EBITDA]), SUM(Financial[Revenue]))

Net Cash = 
SUM(Financial[Cash Inflows]) - SUM(Financial[Cash Outflows])
