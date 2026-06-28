# Indian Banking Sector Comparative Analysis (FY2024)

A comparative financial analysis of 5 major Indian banks across 8 key banking KPIs, built in Excel with an automated ranking scorecard and visual dashboard.

## Overview

This project benchmarks HDFC Bank, ICICI Bank, SBI, Axis Bank, and Kotak Mahindra Bank on the core metrics used to evaluate bank performance — profitability, asset quality, capital strength, and funding cost — and identifies the strongest overall performer using a rank-based scorecard.

## Banks compared

HDFC Bank · ICICI Bank · State Bank of India (SBI) · Axis Bank · Kotak Mahindra Bank

## Methodology

1. **Data collection** — FY2024 figures sourced from company annual reports and screener.in
2. **KPI selection** — 6 ratio metrics plus 2 scale metrics:
   - NIM (Net Interest Margin)
   - Net NPA Ratio
   - ROE (Return on Equity)
   - CAR (Capital Adequacy Ratio)
   - CASA Ratio
   - ROA (Return on Assets)
   - Net Profit (₹ Cr)
   - Total Assets (₹ Cr)
3. **Conditional formatting** — colour-scaled each metric (green = best, red = worst) for instant visual comparison
4. **Ranking scorecard** — ranked each bank 1 (best) to 5 (worst) on every metric, then summed ranks into an overall score (lower total = stronger overall performer)
5. **Verdict formula** — used `INDEX`/`MATCH` to automatically surface the top-ranked bank from the scorecard

## Key results

| Bank | NIM Rank | NPA Rank | ROE Rank | CAR Rank | CASA Rank | ROA Rank | **Overall Score** |
|---|---|---|---|---|---|---|---|
| Kotak Bank | 1 | 1 | 4 | 1 | 1 | 1 | **9** |
| ICICI Bank | 2 | 3 | 2 | 4 | 3 | 2 | 16 |
| Axis Bank | 3 | 2 | 3 | 4 | 2 | 4 | 18 |
| HDFC Bank | 4 | 1 | 5 | 2 | 5 | 3 | 20 |
| SBI | 5 | 5 | 1 | 5 | 4 | 5 | 25 |

**Best overall performer: Kotak Mahindra Bank** — leads on profitability (NIM, ROA) and capital strength (CAR), while SBI's scale advantage comes with weaker efficiency metrics, a common trade-off for India's largest PSU bank.

## Tech stack

- Microsoft Excel (formulas, conditional formatting, charts — no macros)
- Source data: company annual reports, [screener.in](https://www.screener.in)

## Repository contents

| File | Description |
|---|---|
| `Indian_Banking_Comparison.xlsx` | Full workbook — Raw Data, Calculation_sheet (ranked KPIs), and Dashboard (charts + scorecard) |

## How to use

Open `Indian_Banking_Comparison.xlsx` in Excel. The **Dashboard** sheet contains all 4 comparison charts (NIM, NPA, ROE vs ROA, CASA) plus the overall scorecard table. The **Calculation_sheet** has the full ranked metric table with conditional formatting if you want to inspect the underlying ranking logic.

## Notes & limitations

- FY2024 figures are a single-year snapshot; a multi-year trend view (3–5 years) would show whether rankings are stable or shifting
- Equal weighting was used across all 6 ranked metrics — a real research analyst might weight profitability metrics more heavily than capital ratios depending on the use case
- This is an educational/portfolio exercise, not investment advice
