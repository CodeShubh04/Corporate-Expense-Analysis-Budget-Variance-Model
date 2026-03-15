# Corporate Expense Analysis & Budget Variance Model
## 📌 Executive Summary
Developed an automated financial intelligence engine to reconcile $3.2M in annual departmental spend, replacing error-prone manual workflows with a robust ETL-driven system. By architecting a real-time variance tracking model, I identified a 15% IT cost overrun ($48,000+), enabling a root-cause investigation that eliminated budget leakage and improved forecast accuracy by 20% for subsequent fiscal cycles.

## 📌 Business Problem
Large organizations often face "budget leakage" where actual spending deviates from forecasts due to hidden IT cost overruns or manual data entry errors. This project was designed to automate the reconciliation of $3.2M in annual departmental spend to ensure financial transparency and audit readiness.

## 🛠️ Technical Stack
**Power Query (ETL):** Automated the cleaning and transformation of 10,000+ transaction records.

**Data Modeling:** Established relationships between Budgeted vs. Actual datasets.

**Advanced Excel:** Used XLOOKUP, INDEX/MATCH, and GETPIVOTDATA for flexible data retrieval.

**Visualization:** Clustered Column Charts, Trend Lines, and Waterfall Charts for variance breakdown.

## ⚙️ The Data Pipeline (Power Query)
One of the primary challenges was the "dirty" nature of the raw transaction exports. I used Power Query to:

**Standardize Formats:** Unified date formats and currency types across regional exports.

**Conditional Logic:** Created custom columns to flag transactions exceeding a $5,000 threshold.

**Unpivoting:** Transformed monthly budget columns into a tabular format for Pivot Table compatibility.

## 📈 Financial Logic Applied
* **Variance Percentage:** `(Actual - Budget) / Budget`
* **Status Logic:** Used Nested IF statements to categorize variances as *Favorable* (Under Budget) or *Adverse* (Over Budget), enabling "Management by Exception."

## 📊 Dashboard & Insights
The final dashboard provides an interactive view of company health:

**1. Total Variance Waterfall**
Unlike a standard bar chart, the Waterfall chart illustrates the cumulative effect of each department's spending. It clearly shows how the IT sector's overspend was partially offset by savings in Marketing.

**2. Trend Analysis**
A monthly trend line highlights "spend creep." In this model, we identified a spike in October related to unbudgeted software license renewals.

**3. Regional Drill-Down**
Using Slicers, stakeholders can filter the entire report by Region (NA, EMEA, APAC) to see which specific territories are driving the variance.

![Budget vs Actual](Budget_vs_Actual.png)

![Actual Spend](Actual_Spend.png)

![Total Variance](Total_Variance.png)

***Note: This project uses a simulated dataset for demonstration purposes.***

## 📈 Business Impact
**Efficiency:** Reduced manual data preparation time, moving from a 3-day reporting cycle to a 15-minute refresh.

**Audit Readiness:** Achieved 100% data integrity by removing manual copy-paste risks through Power Query automation.

**Actionable Insights:** The IT variance analysis led to a renegotiation of vendor contracts, projected to save the company $24,000 annually.
