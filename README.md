# 🏥 Square Pharmaceuticals PLC — Full Equity Valuation Report
### `DSE: SQURPHARMA` | Analyst: *Your Name* | Date: May 2026

<p align="center">
  <img src="https://img.shields.io/badge/Language-Python_3-blue?style=for-the-badge&logo=python" />
  <img src="https://img.shields.io/badge/Platform-Google_Colab-orange?style=for-the-badge&logo=googlecolab" />
  <img src="https://img.shields.io/badge/Exchange-Dhaka_Stock_Exchange-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Methods-12_Valuation_Models-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge" />
</p>

---

## 📌 Project Overview

This project presents a **comprehensive, multi-method equity valuation** of **Square Pharmaceuticals PLC**, the largest pharmaceutical company listed on the **Dhaka Stock Exchange (DSE)**. Using 10 years of audited financial data (FY2015–FY2025), this notebook applies **12 rigorous valuation and analytical frameworks** rooted in both classical finance theory and statistical modelling.

> **Bottom Line:** The weighted average intrinsic value is estimated at **BDT 270–290 per share**, representing a **~30% upside** over the current market price of BDT 209.

---

## 🎯 Valuation Verdict

| Method | Intrinsic Value (BDT) | vs. Market Price |
|---|---|---|
| DCF — Base Case | ৳225 – ৳230 | +8% to +10% ✅ |
| Dividend Discount Model (2-Stage) | ৳171 – ৳198 | -8% to -18% ⚠️ |
| Peer Multiples — DSE Comps | ৳300 – ৳575 | +44% to +175% 🚀 |
| Monte Carlo Simulation (mean) | ৳231 | +11% ✅ |
| Altman Z-Score | **SAFE ZONE** | ✅ Financially Healthy |
| 🏆 **Weighted Average** | **৳270 – ৳290** | **+30% Upside** |

---

## 🧰 Valuation Methods Used

| # | Method | Tools / Concepts |
|---|---|---|
| 1 | **Exploratory Data Analysis (EDA)** | Descriptive stats, skewness, kurtosis, CV |
| 2 | **Log-Linear OLS Regression** | Revenue & profit trend, R², CAGR |
| 3 | **WACC via CAPM** | Risk-free rate, Beta, Country Risk Premium |
| 4 | **DCF — Discounted Cash Flow** | 5-year FCF projection, terminal value |
| 5 | **DCF Sensitivity Analysis** | 25-scenario WACC × Terminal Growth matrix |
| 6 | **Dividend Discount Model (DDM)** | Gordon Growth + 2-Stage DDM |
| 7 | **Relative Valuation** | P/E, EV/EBITDA, P/B, P/S vs DSE & Asian peers |
| 8 | **DuPont Analysis** | ROE decomposition: Margin × Turnover × Leverage |
| 9 | **Monte Carlo Simulation** | 10,000 DCF runs, probabilistic price distribution |
| 10 | **Altman Z-Score** | Financial distress / bankruptcy risk test |
| 11 | **Correlation Heatmap** | Inter-variable financial relationships |
| 12 | **Valuation Bridge** | Weighted synthesis of all methods |

---

## 📊 Key Financial Highlights (FY2015–FY2025)

- 📈 **Revenue CAGR:** ~10.5% over 10 years
- 💰 **Net Profit CAGR:** ~9.8%
- 🧾 **EPS Growth:** Consistent upward trend
- 🏦 **Zero Debt:** Net cash positive company
- 💵 **FCF Base (FY2026E):** BDT 18,200 million
- 🔒 **Altman Z-Score:** Safe zone — no financial distress risk
- 📉 **WACC Used:** ~15% (Bangladesh CAPM + Country Risk Premium)

---

## 🗂️ Project Structure

```
SquarePharma_Valuation.ipynb
│
├── Step 0  — Library Installation & Imports
├── Step 1  — 10-Year Financial Dataset (FY2015–FY2025)
├── Step 2  — EDA: Descriptive Stats + Correlation Heatmap
├── Step 3  — OLS Regression & CAGR Estimation
├── Step 4  — WACC Calculation (CAPM + Country Risk Premium)
├── Step 5  — DCF Valuation
├── Step 6  — DCF Sensitivity Matrix (5×5)
├── Step 7  — Dividend Discount Model (Gordon + 2-Stage)
├── Step 8  — Relative Valuation (Peer Multiples)
├── Step 9  — DuPont Analysis
├── Step 10 — Monte Carlo Simulation (10,000 runs)
├── Step 11 — Altman Z-Score
└── Step 12 — Valuation Bridge & Final Synthesis
```

---

## ⚙️ Tech Stack

```python
numpy          # Numerical computation
pandas         # Financial data manipulation
matplotlib     # Custom financial charts
seaborn        # Correlation heatmap
scipy          # Statistical tests (skewness, kurtosis, normality)
statsmodels    # OLS regression (log-linear trend analysis)
openpyxl       # Excel data support
```

---

## 🚀 How to Run

### Option 1 — Google Colab (Recommended)
1. Click the badge below to open directly in Colab:

   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_vrImCv6UFi7VsztTuZGY4UpAqEe_hSc)

2. Go to **Runtime → Run All**
3. All libraries are auto-installed in the first cell

### Option 2 — Local Jupyter
```bash
git clone https://github.com/AbdullahAlForman/squarepharma-valuation.git
cd squarepharma-valuation
pip install numpy pandas matplotlib seaborn scipy statsmodels openpyxl
jupyter notebook SquarePharma_Valuation.ipynb
```

---

## 📚 Data Sources

- Square Pharmaceuticals PLC Annual Reports (2015–2025) — [squarepharma.com.bd](https://squarepharma.com.bd)
- Dhaka Stock Exchange (DSE) historical price data
- Bangladesh Bank — Government T-bill yield (risk-free rate)
- Damodaran — Equity Risk Premium & Country Risk Premium databases

---

## 🔑 Key Assumptions

| Parameter | Value | Rationale |
|---|---|---|
| Risk-Free Rate (Rf) | 8.75% | Bangladesh Govt bond yield |
| Equity Risk Premium | 6.00% | Mature market base |
| Country Risk Premium | 2.50% | Bangladesh sovereign risk |
| FCF Growth Rate | 11% | Conservative vs 10-yr CAGR |
| Terminal Growth Rate | 5.00% | GDP + inflation adjusted |
| Projection Period | 5 Years | Standard DCF horizon |

---

## ⚠️ Disclaimer

> This project is for **academic and educational purposes only**. It is not investment advice. All data is sourced from publicly available documents. The author is not responsible for any financial decisions made based on this analysis.

---

## 👤 Author

**[Your Name]**  
BBA (Finance) — University of Dhaka  
📧 datascience189@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/yourprofile) | [GitHub](https://github.com/AbdullahAlForman)

---

## ⭐ If you found this useful, please star the repo!

<p align="center">
  Made with ❤️ in Dhaka, Bangladesh 🇧🇩
</p>
