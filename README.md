# Rockbound 2050 Global Market Portfolio — interactive chart

Streamlit app behind the "Explore Interactive Chart" button on
www.rockbound-capital.com/investment-strategy. Plots the growth of $10,000
in the Rockbound 2050 Global Market Portfolio against the Vanguard Target
Retirement 2050 Fund and the S&P 500 (dividends reinvested), with a date
range slider and per-series performance metrics.

## Data

`values.csv` holds month-end portfolio values rebased to $10,000 at the
common start (January 2021). It is regenerated and pushed by
`scripts/make_website_charts.sh` in the `actions-rockbound-results` repo —
the same run that produces the website's chart images — so the app and the
website can never show different data. Streamlit Community Cloud redeploys
automatically on every push.

## Run locally

```
pip install -r requirements.txt
streamlit run streamlit_app.py
```
