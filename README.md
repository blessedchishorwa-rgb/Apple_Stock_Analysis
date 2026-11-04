# Apple Stock Performance and Risk Analysis

## Project Overview

This project analyzes Apple Inc. (AAPL) stock performance from 21 October 2024 to 16 October 2026 using an end-to-end data analytics workflow. It combines Excel and Power Query for data preparation, SQL for querying and validation, Python for automated analysis and visualization, and Power BI for interactive dashboard reporting.

The central business question was:

> How did Apple’s stock price perform over the selected two-year period, and how volatile was that performance?

## Tools Used

| Tool | Purpose |
|---|---|
| Excel and Power Query | Imported, cleaned, filtered, and analyzed the historical price data |
| SQL | Queried the dataset and calculated returns, moving averages, and summary statistics |
| Python | Automated calculations, created reproducible charts, and validated results |
| Power BI | Built an interactive dashboard with KPIs, filters, and trend visuals |
| GitHub | Organized and presented the project as a portfolio case study |

## Dataset

The dataset contains Apple’s daily stock market data, including:

- Date
- Open price
- High price
- Low price
- Closing price
- Trading volume
- Daily return
- 30-day moving average

The analysis period covers 21 October 2024 to 16 October 2026. The first available trading date in the filtered dataset was 21 October 2024, and the final available trading date was 16 October 2026.

## Methodology

1. Imported Apple’s historical price data into Excel.
2. Used Power Query to create a separate two-year analysis dataset while preserving the full historical dataset.
3. Filtered the data from 20 October 2024 to 19 October 2026.
4. Calculated daily percentage returns.
5. Calculated a 30-day moving average.
6. Calculated summary risk and return measures.
7. Recreated and validated the analysis in SQL and Python.
8. Built an interactive Power BI dashboard.

## Formulas

**Daily Return**

Daily Return = (Today’s Close − Previous Close) ÷ Previous Close

**Annualized Volatility**

Annualized Volatility = Daily Standard Deviation × √252


**Cumulative Return**

Cumulative Return = (Last Closing Price ÷ First Closing Price) − 1

The value 252 represents the approximate number of trading days in a year.

## Key Results

| Measure | Result |
|---|---:|
| Analysis start date | 21 October 2024 |
| Analysis end date | 16 October 2026 |
| First closing price | 113.055 |
| Last closing price | 343.46 |
| Cumulative return | 203.73% |
| Average daily return | 0.09% |
| Daily standard deviation | 1.75% |
| Annualized volatility | 27.80% |
| Best daily return | 15.33% |
| Worst daily return | -9.25% |

## Key Insights

- Apple’s stock price increased from 113.055 to 343.46 during the two-year analysis period.
- The cumulative return of approximately 203.73% means Apple’s closing price more than tripled.
- The positive average daily return of 0.09% shows that, on average, Apple’s price increased slightly on each trading day.
- Annualized volatility of 27.80% shows that Apple experienced meaningful short-term price fluctuations.
- The best daily return was 15.33%, while the worst daily return was -9.25%.
- The 30-day moving average confirms that Apple’s broader trend was upward despite short-term declines.
- The Power BI dashboard makes the analysis interactive and allows users to explore performance across different date ranges.

## SQL Analysis

The SQL file, `sql/apple_analysis.sql`, contains queries for:

- Creating the `apple_prices` table
- Importing the cleaned CSV dataset
- Calculating daily returns
- Calculating the 30-day moving average
- Filtering the two-year analysis period
- Calculating cumulative return
- Identifying the best and worst trading days
- Calculating monthly average returns
- Creating a price trend view

## Python Analysis

The Python notebook, 'notebooks/apple_analysis.ipynb`, performs the following tasks:

- Loads and cleans the Apple price dataset
- Calculates daily returns
- Calculates the 30-day moving average
- Calculates average daily return, volatility, annualized volatility, and cumulative return
- Creates closing-price and daily-return visualizations
- Validates the results produced in Excel and SQL

## Power BI Dashboard

The Power BI dashboard includes two pages:

1. Performance Overview — KPI cards, closing-price trend, 30-day moving average, and date filter.
2. Risk and Returns — daily returns, monthly returns, and detailed price and return data.

The dashboard allows users to filter the analysis by date and explore Apple’s performance across the selected period.

## Limitations

- The analysis is based on historical data and does not predict future stock performance.
- Returns are calculated using closing prices and do not include dividends unless the source data is dividend-adjusted.
- The fixed two-year period may not represent Apple’s performance during different market conditions.
- Volatility is estimated using historical daily returns and may change in the future.
- The analysis focuses on one stock and does not compare Apple’s performance with competitors, market indexes, or risk-free investments.

## Full Report

View the complete Notion report here: [Apple Stock Performance And Risk Analysis](https://www.notion.so/Apple-Stock-Performance-and-Risk-Analysis-Excel-SQL-Python-Power-BI-3efd7f269d0f802dbe03fd8540b8c3c9)
