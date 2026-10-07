# 💸 SmartSpend AI

**Track. Understand. Detect. Save.**
Intelligent expense management and anomaly detection for your **home** and your **business**. Built for the IEEE Day Vibe Coding competition.

## Features
- **Two workspaces:** Home and Business, each with its own expenses, budgets and categories
- **Dashboard:** total spending, budget, remaining budget, anomalies, trend, category split, recent transactions, projected month-end spend and Spend Control Score
- **Expenses:** add, search, filter, delete, automatic categorization, CSV import and export
- **Analytics:** monthly, weekday and category breakdowns
- **Anomaly detection:** per-category statistical outliers (mean + 2σ and at least 1.8× typical) and duplicate same-day charges
- **Budgets:** per-category limits, alerts at 80% and when exceeded, budget CSV import
- **AI insights:** rule-based insights and a next-month plan to trim spending
- **Notifications:** budget, anomaly and projection alerts
- **PDF report:** summary, budget vs actual, insights, anomalies, trim plan and recent expenses
- **Demo mode** with realistic sample data
- **Responsive**, dark-first design with a light theme

## Tech
Single-file app: HTML, CSS and vanilla JavaScript. Charts are hand-drawn SVG and PDFs use [jsPDF](https://github.com/parallax/jsPDF) loaded from cdnjs. Data is stored in the browser's `localStorage`. There is no backend.

## Run locally
Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy on GitHub Pages
1. Push this repo to GitHub.
2. Go to **Settings → Pages → Source: GitHub Actions**.
3. Every push to `main` deploys the site automatically.

## CSV formats
- Expenses: `date,description,amount[,category]` with dates as `YYYY-MM-DD`
- Budgets: `category,limit`

## Limitations and roadmap
- Sign-in is a local profile only, with no password or server
- Insights are rule-based, not from a language model
- Planned: Replit/Node backend with a database and auth, real LLM insights, combined Home + Business view, multi-currency

## License
MIT
