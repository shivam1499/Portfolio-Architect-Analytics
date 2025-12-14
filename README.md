# Portfolio Architect: A Data-Driven Framework for Analyzing Global vs. Canadian Sector Performance

![Python](https://img.shields.io/badge/Python-3.11-blue.svg) 
![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20Prophet%20%7C%20yfinance-orange.svg) 
![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-yellow.svg)

This capstone project is a full-stack data analytics solution designed to analyze the performance, risk, and diversification trade-offs between Canadian "home-country" biased portfolios and globally diversified ones. The repository contains the complete Python script for the ETL pipeline and machine learning forecasting, along with the final Power BI report that serves as the interactive front-end.
---

## 1. Business Problem & Solution

The Canadian equity market (S&P/TSX) is structurally concentrated in the Financials and Energy sectors. This project addresses the key problems stemming from this "home-country bias," namely a lack of diversification, missed global growth opportunities (especially in Technology), and an absence of data-driven tools for financial advisors.

The **"Portfolio Architect"** solution provides a quantitative framework to address these issues. It uses an automated Python pipeline to process historical data and a Prophet ML model to generate forecasts, with all insights delivered through a dynamic, 4-page Power BI dashboard.

---

## 2. Key Features

*   **Automated ETL Pipeline:** A Python script that programmatically extracts historical daily market data for six sector ETFs from the Yahoo Finance API, ensuring data is always current.
*   **Methodological Soundness:** Enforces a strict "apples-to-apples" comparison by automatically aligning all ETF data to a common start date, a critical step for accurate historical analysis.
*   **Machine Learning Forecasting:** Implements the **Facebook Prophet** model to generate 30-day forward-looking price forecasts, complete with confidence intervals, for each sector.
*   **Advanced BI Dashboard:** The solution culminates in a 4-page, interactive Power BI report built on a best-practice **Star Schema** data model.
*   **Dynamic "What-If" Analysis:** Includes a **Portfolio Simulator** page where users can interactively adjust the allocation between Canadian and Global assets to see the real-time impact on a portfolio's return, risk, and Sharpe Ratio.
*   **Prescriptive Analytics:** The dashboard automatically calculates and recommends the optimal portfolio allocation that would have historically yielded the best risk-adjusted return.

---

## 3. Technology Stack & Architecture

*   **Data Engineering & ML:** Python (Pandas, NumPy, yfinance, Prophet)
*   **Data Modeling:** Power Query (Data Shaping, Unpivoting), Star Schema
*   **Calculation Engine:** Advanced DAX (Dynamic Measures, Time Intelligence, Simulation Formulas)
*   **Data Visualization:** Microsoft Power BI (Line Charts, Scatter Plots, Heatmaps, AI Visuals)

---

## 4. How to Use This Project

This project consists of a Python backend for data processing and a Power BI frontend for visualization.

**Step 1: Run the Python Backend**
1.  Ensure you have all necessary libraries installed by running `pip install -r requirements.txt`.
2.  Execute the main Python script (`main_analysis.py`).
3.  The script will generate a suite of clean CSV files (e.g., `adj_close_prices.csv`, `summary_metrics.csv`, `combined_forecasts_all_etfs.csv`) in the `output_data` folder. These files are the data source for the Power BI report.

**Step 2: Use the Power BI Frontend**
1.  Open the `Portfolio_Architect_Dashboard.pbix` file in Power BI Desktop.
2.  If prompted, you may need to update the data source path to point to the folder where your CSV files were saved.
3.  Refresh the data to ensure the report is using the latest outputs from the Python script.
4.  Interact with the 4-page dashboard using the custom navigation and the filter pane on the right.

---

## 5. Dashboard Preview

•	![The Executive Dashboard ](https://github.com/shivam1499/Portfolio-Architect-Analytics/blob/8acb8fae2cd66e7694587cc83adbdd3909755be2/Executive%20Dashbaord.JPG)

•	![The Portfolio Simulator & Forecast](https://github.com/shivam1499/Portfolio-Architect-Analytics/blob/main/Simulator.JPG)

•	![The Performance Page](https://github.com/shivam1499/Portfolio-Architect-Analytics/blob/main/Performance%20Deep%20dive.JPG)

•	![The Risk & Diversification](https://github.com/shivam1499/Portfolio-Architect-Analytics/blob/main/Risk%20and%20Diversification.JPG)
 
•	![The About](https://github.com/shivam1499/Portfolio-Architect-Analytics/blob/main/About.JPG)

 
---

## 6. Author(s) & Acknowledgments

This project was developed as a capstone for the Business Insights and Analytics program at Humber College.

*   **Team:** Hevisaben Patel, Shivam Patidar, Divika Tapaswi, Pushkar Pradhan, Shikha Patel, Krishna Gandhi
*   **Guidance:** Professor Omar Wahdan
