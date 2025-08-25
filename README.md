## Financial Market Prep Data Engineering Project

This project contains a Python-based data engineering pipeline to construct a historical financial dataset for investment backtesting. It uses the Financial Modeling Prep (FMP) API to gather data.

### Objective

The goal is to create two datasets for companies that have had a market capitalization of over $100 million in the last 10 years:

1.  **Quarterly Total Return Stock Prices**: A dataset of end-of-quarter stock prices for the last 10 years, adjusted for splits, dividends, and other corporate actions to reflect total returns.
2.  **Point-in-Time Fundamental Metrics**: A dataset of key financial metrics (assets, debt, revenue, EPS, employee count) as they were reported, along with company metadata (country, sector, industry).

### Structure

-   `data_pipeline/`: Main source code directory.
    -   `main.py`: The entry point for running the data pipeline.
-   `requirements.txt`: Project dependencies.
-   `output/`: Directory where the final CSV datasets will be saved.

### How to Run

1.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
2.  Set your FMP API key as an environment variable:
    ```bash
    export FMP_API_KEY='your_api_key'
    ```
3.  Run the main script:
    ```bash
    python data_pipeline/main.py
    ```
