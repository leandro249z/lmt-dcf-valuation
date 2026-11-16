# lmt-dcf-valuation
Lockheed Martin DCF valuation in Excel: WACC, terminal value, equity bridge, and sensitivity analysis from FY2025 filings
    # Lockheed Martin (LMT) Discounted Cash Flow Valuation

**File:** `LMT_DCF_Model.xlsx`

I valued Lockheed Martin using a discounted cash flow (DCF) model. I chose it because it is a large aerospace and defense company, which makes it a good example of the program-finance work I want to do.

### Result

| Metric | Value |
|---|---|
| Implied value per share (base case) | about $480 |
| Share price used (Oct 30, 2026 close) | $636.95 |
| Implied upside / (downside) | about (25%) |
| WACC | 7.6% |
| Terminal growth | 2.5% |
| Terminal value as % of enterprise value | 79% |
| Implied terminal EV / EBITDA | 12.5x |
| Current EV / EBITDA (2025) | 17.5x |

At these assumptions, the model values LMT below the market price. The market is pricing in higher growth, higher margins, or a lower discount rate than my base case. I think that gap is the most useful part of the analysis, not the single number.

### What the model contains

- **Summary:** key outputs and how to read them
- **Inputs:** market data, WACC inputs and forecast assumptions
- **Historicals:** FY2024 and FY2025 financials from Lockheed Martin's earnings release, with ratios calculated by formula
- **DCF:** five-year forecast (2026E–2030E), unlevered free cash flow, discounting, terminal value and equity bridge
- **Sensitivity:** implied value per share across a range of WACC and terminal growth rates
- **Sources:** where every sourced number came from

Every number from a filing is typed in blue and traces to a source. Every calculation is a live formula, so the model updates if an input changes. Assumptions are highlighted in yellow.

### Sources

- Lockheed Martin, *Reports Fourth Quarter and Full Year 2025 Financial Results* (January 29, 2026): sales, operating profit, interest expense, taxes, EPS, cash flow, capex, debt, cash and equity
- StockAnalysis (stockanalysis.com/stocks/lmt): share price (Oct 30, 2026 close) and shares outstanding
- YCharts: 10-year U.S. Treasury yield, 5.10% (Nov 12, 2026)

### My assumptions (not sourced)

| Input | Value | Why |
|---|---|---|
| Equity risk premium | 5.0% | Within the commonly used 4–6% range |
| Beta | 0.60 | Judgment call. The data site showed 0.10, which looked too low to trust. |
| Revenue growth | 4.9% fading to 3.0% | Starts near the midpoint of 2026 sales guidance ($77.5–80.0B) |
| Operating margin | 10.6% flat | 2025 actual was 10.3%. Company guidance implies a higher non-GAAP segment margin. |
| Capex % of sales | 3.4% fading to 3.0% | Starts near 2026 capex guidance ($2.5–2.8B) |
| D&A % of sales | 2.25% | Close to the 2025 actual of 2.2% |
| Working capital | 5% of added revenue | Simple placeholder. I did not pull detailed working-capital data. |
| Terminal growth | 2.5% | Should not exceed long-run economic growth |

### Limitations

- **Pension obligations are not modeled.** Lockheed has large pension liabilities and a large 2025 non-service pension swing, so this is the biggest gap.
- **Leases and other debt-like items are excluded** from net debt.
- **Timing mismatch:** cash flows are discounted from December 31, 2025, but compared with an October 2026 share price. A full model would roll the valuation date forward.
- **Beta is a judgment call.** A regression against the S&P 500 over five years would be a better estimate.
- **No scenarios.** The model does not test defense budget changes, program risk (such as the F-35), or contract charges.

### What I would improve next

1. Model pension obligations as debt-like items
2. Estimate beta from a regression instead of using a judgment value
3. Add bull, base and bear scenarios
4. Pull FY2023 data to show a longer history

---

I built this to practice the valuation skills used in corporate finance, FP&A and financial risk. I work in financial reporting and investment analysis at La Fábrica PR LLC, and I am completing my B.B.A. in Finance at the University of Puerto Rico, Mayagüez campus. I would welcome feedback.

    

