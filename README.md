# Indian Banking Financial & Risk Analysis (FY2021–FY2025)

## 📌 Project Overview
An end-to-end financial performance, econometric validation, and credit risk assessment project evaluating the 5-year trajectory (**FY2021–FY2025**) of five major Indian banks: **State Bank of India (SBI), HDFC Bank, ICICI Bank, Axis Bank, and Bank of Baroda**[cite: 2, 12].

The workflow integrates exploratory data analysis, financial ratio engineering, OLS regression diagnostics, and multi-factor risk scoring in **Python**, relational storage in **SQLite**, and interactive executive reporting in **Microsoft Power BI**[cite: 1, 2, 3, 12].

---

## 📂 Repository Structure
* **`Project_1_Banking_Data.xlsx`** – Raw 5-year financial dataset (FY2021–FY2025) covering Deposits, Advances, Total Assets, Net Profit, ROA, ROE, GNPA, NNPA, CAR, NIM, Provision Coverage Ratio, and Cost/Income Ratio[cite: 2, 11].
* **`Project_1_Banking_Analysis.ipynb`** – Complete Jupyter Notebook containing EDA, YoY growth trends, correlation analysis, OLS regression diagnostics (VIF, Breusch-Pagan, Jarque-Bera, Durbin-Watson), composite risk scoring, and 20 visualizations[cite: 2, 11, 12, 13].
* **`final_banking_dataset.csv` & `banking_analysis.xlsx`** – Processed datasets enriched with engineered financial ratios, period-over-period changes, and risk metrics[cite: 11].
* **`project_1_banking.db`** – SQLite database (`bank_data` table) storing the final scored dataset (`GNPA_Risk`, `NNPA_Risk`, `ROA_Risk`, `CAR_Risk`, and `Risk_Score`)[cite: 1, 11].
* **`Banking_Analysis_Dashboard.pbix`** – Interactive 4-page Power BI executive dashboard for visual benchmarking across banks and financial years[cite: 3, 11].
* **`images/`** – Folder containing all **20 exported Matplotlib plots** covering growth trajectories, asset quality, capital adequacy, OLS residual diagnostics, and banking risk scorecards[cite: 13].

---

## 📈 All 20 Visuals & Charts

### Part 1: Initial Trend Exploration (Step 9)
| SBI Net Profit Trend | Net Profit Comparison |
| :---: | :---: |
| ![SBI Net Profit Trend](images/chart_01_cell5.png) | ![Net Profit Trend](images/chart_02_cell5.png) |

| GNPA Trend (Raw Scale) | ROA Trend (Raw Scale) |
| :---: | :---: |
| ![GNPA Trend](images/chart_03_cell5.png) | ![ROA Trend](images/chart_04_cell5.png) |

---

### Part 2: Comparative Growth, Solvency & Asset Quality (Step 12)
| Net Profit Trend | Advances Growth (%) |
| :---: | :---: |
| ![Net Profit Comparison](images/chart_05_cell8.png) | ![Advances Growth](images/chart_06_cell8.png) |

| GNPA Trend | ROA Trend |
| :---: | :---: |
| ![GNPA Comparison](images/chart_07_cell8.png) | ![ROA Comparison](images/chart_08_cell8.png) |

| Capital Adequacy Ratio (CAR) Trend | GNPA vs. ROA Scatter |
| :---: | :---: |
| ![CAR Trend](images/chart_09_cell8.png) | ![GNPA vs ROA](images/chart_10_cell8.png) |

---

### Part 3: Econometric Regression Diagnostics (Step 19)
| OLS Residuals vs. Predicted ROA |
| :---: |
| ![Residuals vs Predicted ROA](images/chart_11_cell15.png) |

---

### Part 4: Final Banking Risk Dashboard Charts (Step 23)
| Net Profit Trend (Styled) | GNPA Trend (%) |
| :---: | :---: |
| ![Final Net Profit Trend](images/chart_12_cell19.png) | ![Final GNPA Trend](images/chart_13_cell19.png) |

| ROA Trend (%) | Capital Adequacy Ratio (%) |
| :---: | :---: |
| ![Final ROA Trend](images/chart_14_cell19.png) | ![Final CAR Trend](images/chart_15_cell19.png) |

| Average Composite Risk Score by Bank | Average Advances-to-Deposits Ratio (%) |
| :---: | :---: |
| ![Average Risk Score](images/chart_16_cell19.png) | ![Advances to Deposits Ratio](images/chart_17_cell19.png) |

| GNPA (%) vs. ROA (%) Correlation | SBI Net Profit Summary |
| :---: | :---: |
| ![Final GNPA vs ROA](images/chart_18_cell19.png) | ![SBI Net Profit Summary](images/chart_19_cell23.png) |

| All Banks Net Profit Summary |
| :---: |
| ![All Banks Net Profit Summary](images/chart_20_cell23.png) |

---

## 📊 Financial & Risk Framework
* **Growth & Scale Metrics:** Year-over-Year (YoY) and 5-year cumulative growth across Net Profit, Deposits, Advances, and Total Assets[cite: 2].
* **Profitability & Efficiency:** Return on Assets (ROA), Return on Equity (ROE), Net Interest Margin (NIM), Cost-to-Income Ratio, and Profit-to-Advances Ratio[cite: 2].
* **Liquidity & Solvency:** Advances-to-Deposits Ratio (CDR) and Capital Adequacy Ratio (CAR)[cite: 2].
* **Econometric Validation:** Multiple OLS regression modeling ROA against GNPA, CAR, and NIM, validated via Variance Inflation Factor (VIF), Breusch-Pagan heteroscedasticity test, Jarque-Bera normality test, and Durbin-Watson autocorrelation diagnostics[cite: 12].
* **Composite Risk Scoring:** Min-max normalized risk indicators (`GNPA_Risk`, `NNPA_Risk`, `ROA_Risk`, `CAR_Risk`) combined into an equal-weighted **`Risk_Score`** per bank and financial year[cite: 1, 12].

---

## 🔍 Key Analytical Insights (FY2021–FY2025)
1. **Sector-Wide Asset Quality Turnaround:** All five banks substantially reduced Gross NPAs over the 5-year period[cite: 2]. **Bank of Baroda** recorded the sharpest turnaround, lowering GNPA by **6.07 percentage points** (from **8.87%** in FY2021 to **2.80%** in FY2025)[cite: 2].
2. **Profitability Leaders:** **ICICI Bank** achieved the highest 5-year average ROA (**2.00%**) and ROE (**16.26%**), scaling Net Profit by **236.3%** (from ₹16,193 Cr to ₹54,449 Cr)[cite: 2]
