# Indian Banking Financial & Risk Analysis (FY2021–FY2025)

## 📌 Project Overview
An end-to-end financial performance and credit risk assessment project evaluating the 5-year trajectory (**FY2021–FY2025**) of five major Indian banks: **State Bank of India (SBI), HDFC Bank, ICICI Bank, Axis Bank, and Bank of Baroda**[cite: 2].

The pipeline integrates data cleaning, ratio engineering, and multi-factor risk scoring in **Python**, relational storage in **SQLite**, and interactive visual reporting in **Microsoft Power BI**[cite: 1, 2, 3].

---

## 📂 Repository Files
* **`Project_1_Banking_Data.xlsx`** – Raw 5-year financial dataset (FY2021–FY2025) containing Deposits, Advances, Total Assets, Net Profit, ROA, ROE, GNPA, NNPA, CAR, NIM, Provision Coverage Ratio, and Cost/Income Ratio[cite: 2, 10].
* **`Project_1_Banking_Analysis.ipynb`** – Jupyter Notebook covering exploratory data analysis, YoY and 5-year cumulative growth trends, banking risk ratios, correlation analysis, and Matplotlib visualizations[cite: 2, 10].
* **`banking_analysis.xlsx`** – Processed Excel dataset enriched with engineered financial ratios, period-over-period changes, and risk metrics[cite: 10].
* **`banking_analysis.db`** – SQLite database (`bank_data` table) storing the final dataset along with granular and composite risk scores (`GNPA_Risk`, `NNPA_Risk`, `ROA_Risk`, `CAR_Risk`, and `Risk_Score`)[cite: 1, 10].
* **`Banking_Analysis_Dashboard.pbix`** – Interactive 4-page Power BI executive dashboard for visual benchmarking of growth, profitability, asset quality, and risk[cite: 3, 10].

---

## 📊 Financial & Risk Framework
* **Growth & Scale Metrics:** Year-over-Year (YoY) and 5-year cumulative growth across Net Profit, Deposits, Advances, and Total Assets[cite: 2].
* **Profitability & Efficiency:** Return on Assets (ROA), Return on Equity (ROE), Net Interest Margin (NIM), Cost-to-Income Ratio, and Profit-to-Advances Ratio[cite: 2].
* **Liquidity & Solvency:** Advances-to-Deposits Ratio (CDR) and Capital Adequacy Ratio (CAR)[cite: 2].
* **Asset Quality & Composite Risk Scoring:** Evaluation of Gross NPA (GNPA), Net NPA (NNPA), and Provision Coverage Ratio (PCR)[cite: 2], combined with normalized risk components (`GNPA_Risk`, `NNPA_Risk`, `ROA_Risk`, `CAR_Risk`) to compute an overall **`Risk_Score`** per bank and financial year[cite: 1].

---

## 🔍 Key Analytical Insights (FY2021–FY2025)
1. **Sector-Wide Asset Quality Turnaround:** All five banks substantially reduced Gross NPAs over the 5-year period[cite: 2]. **Bank of Baroda** recorded the sharpest turnaround, lowering GNPA by **6.07 percentage points** (from **8.87%** in FY2021 to **2.80%** in FY2025)[cite: 2].
2. **Profitability Leaders:** **ICICI Bank** achieved the highest 5-year average ROA (**2.00%**) and ROE (**16.26%**), scaling Net Profit by **236.3%** (from ₹16,193 Cr to ₹54,449 Cr
