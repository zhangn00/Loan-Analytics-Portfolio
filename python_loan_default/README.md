# Loan Default Risk Analysis (Python)

**Data Source**  
Lending Club Accepted Loans (sample 100k rows, 2007–2018).
https://www.kaggle.com/datasets/wordsforthewise/lending-club/code

**Quick Access** (Google Drive)
https://drive.google.com/drive/folders/1_g8Mikaxehd1_jwzLntvZNxylWA-1j3g
## Objective  
Quantify how borrower characteristics affect default probability and visualize key risk drivers.

## Key Steps  
1. **Data Prep** — select `loan_amnt`, `grade`, `int_rate`, `annual_inc`, `loan_status`.  
2. **Feature Engineering** — `is_default` flag, income quartile buckets, loan amount buckets.  
3. **Descriptive Analytics** — five chart outputs in `output/`:

| Chart | Insight |
|-------|---------|
| `default_rate_by_grade.png` | Default ↑ from 5 % (Grade A) → 50 % (Grade G) |
| `default_rate_by_income.png` | Low-income quartile default ≈ 20 %, top quartile ≈ 14 % |
| `int_rate_by_grade.png` | Avg rate climbs from 6 % (A) → 27 % (G) |
| `int_rate_boxplot_by_grade.png` | Distribution widens for lower grades, showing higher pricing dispersion |
| `default_rate_by_loan_amt.png` | Loans > 35 k show slightly higher risk (~19 %) |

4. **Optional Model** — baseline logistic regression, AUC = 0.66.

## Repo Layout
