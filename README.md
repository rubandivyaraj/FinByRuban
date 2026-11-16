# FinCal by Ruban

A simple, responsive finance calculator suite in Indian Rupees (INR). It runs as a single HTML file, with no install or build step.

> All results are educational estimates only. They are not actual returns, financial advice, or a guarantee from any bank or investment provider.

## Run locally

1. Download or clone the repo.
2. Open `fincal.html` in any modern browser.

An internet connection is needed for the charts (Chart.js) and the Inter font, which both load from a CDN.

## Calculators

| Tab | What it does |
|-----|--------------|
| **Buy Home** | Home-loan EMI, total interest, total cost of the home and EMI-to-income ratio. An optional yearly extra payment shows interest saved, time saved and the new tenure. |
| **Invest** | Monthly SIP with a yearly step-up, an inflation-adjusted value and a target-amount progress bar. If the target isn't met, it shows the shortfall and the starting SIP needed. |
| **Save** | Fixed deposit with cumulative, monthly or quarterly payout and selectable compounding. It shows tax on interest, post-tax value, effective return and inflation-adjusted value. |
| **Loan** | Personal-loan EMI, total interest, interest as a percentage of the loan, and savings from a yearly extra payment. |

## Features

- Doughnut and line charts for every calculator (Chart.js)
- Light and dark theme that follows your system setting, with a manual toggle
- Inputs, selected tab and theme are saved in your browser (localStorage)
- INR formatting in the Indian numbering system, such as ₹1,00,000
- Negative values are blocked
- Responsive layout for phones, tablets and desktops

## Assumptions

- Loan EMI uses the standard reducing-balance formula. A yearly extra payment is applied at the end of each 12th month.
- FD tax is applied as one charge on total interest at maturity, not year by year.
- The SIP return is compounded monthly, and the step-up applies once a year.
- Inflation-adjusted values divide by compounded yearly inflation.

## Tech

HTML, CSS and vanilla JavaScript, with [Chart.js](https://www.chartjs.org/) loaded from a CDN.

## Disclaimer

FinCal is for education and general planning. Actual bank rates, taxes, fees, compounding rules, investment performance and loan terms may differ. Confirm important decisions with your bank or a qualified financial advisor.
