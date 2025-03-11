# Canadian Banks Stock Data Analysis

## Project Overview

This project aims to analyze the stock performance of major Canadian banks over a specific period. By leveraging historical stock data, we seek to identify trends, assess market volatility, and provide data-driven insights to support informed investment decisions.  
For a detailed analysis, refer to the full report: [Canadian Banks Stock Report](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/blob/main/reports/Canadian_Banks_Stock_Report_draft1.pdf)

### Goals  
- Analyze historical stock price trends for major Canadian banks.  
- Assess market volatility and its impact on stock performance.  
- Identify correlations between stock price movements and external factors.  
- Develop predictive models to forecast future stock prices.  
- Present insights through interactive dashboards and reports.  

### Business Questions  
- What are the key trends in Canadian bank stock performance?  
- How volatile have these stocks been over time?  
- Can we predict future stock performance based on historical data?  
- How do different banks compare in terms of stability and returns?  

By answering these questions, we aim to provide actionable insights for investors and analysts.  

## Repository Structure

- [`data/`](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/tree/main/data): Contains the raw and processed datasets used for analysis.  
- [`notebooks/`](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/tree/main/notebooks): Jupyter notebooks detailing the data cleaning, exploration, and analysis processes.  
- [`dashboard/`](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/tree/main/dashboard): Interactive visualizations and dashboards presenting key findings.  
- [`reports/`](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/tree/main/reports): Generated reports summarizing the analysis and insights.  

[Project Repository](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis)  

## Data Collection  

The dataset comprises historical stock prices for major Canadian banks, sourced through web scraping from [Yahoo Finance](https://ca.finance.yahoo.com/). The data includes stock prices from January 2020 to December 2024, capturing daily closing prices, trading volumes, and other key metrics.  

### Data Source  
Web scraping was used to efficiently and automatically extract stock data, ensuring an up-to-date and comprehensive dataset. The dataset covers the following banks:  

- **[Bank of Montreal (BMO)](https://ca.finance.yahoo.com/quote/BMO.TO/history)**  
- **[Bank of Nova Scotia (BNS)](https://ca.finance.yahoo.com/quote/BNS.TO/history)**  
- **[Canadian Imperial Bank of Commerce (CM)](https://ca.finance.yahoo.com/quote/CM.TO/history)**  
- **[Royal Bank of Canada (RY)](https://ca.finance.yahoo.com/quote/RY.TO/history)**  
- **[Toronto-Dominion Bank (TD)](https://ca.finance.yahoo.com/quote/TD.TO/history)**  

### Data Structure  
The dataset consists of the following columns:  

- **`stock_ticker`** – Bank stock symbol (e.g., BMO.TO, TD.TO)  
- **`date`** – Trading date  
- **`close_price`**, **`high_price`**, **`low_price`**, **`open_price`** – Daily stock prices  
- **`volume`** – Number of shares traded  

These variables are essential for understanding price trends and trading activity.  


## Dashboard

An interactive dashboard is available to visualize key findings from the analysis. The dashboard provides insights into stock trends, volatility, and comparisons among the banks.
![image](https://github.com/user-attachments/assets/82ef8f55-fe2a-4d60-a0b4-73b245522047)
![image](https://github.com/user-attachments/assets/e595c902-46ae-447c-817c-4ba715a25175)

**Access the dashboard here:** [Dashboard Link](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/tree/main/dashboard)

## Key Findings

1. **Stock Performance Trends**: Analysis revealed that all five banks experienced growth in their stock prices over the analyzed period, with notable fluctuations corresponding to major economic events.
2. **Volatility Assessment**: The banks exhibited varying levels of volatility, with some showing more resilience to market downturns than others.
3. **Correlation Analysis**: There is a high positive correlation among the stock prices of these banks, indicating that they often move in tandem, likely due to their exposure to similar market conditions.

## Recommendations

- **Diversification**: Investors should consider diversifying their portfolios to mitigate risks associated with sector-specific downturns.
- **Regular Monitoring**: Given the observed volatility, regular monitoring of stock performance is advisable to make timely investment decisions.
- **Further Research**: Additional analysis incorporating macroeconomic indicators could provide deeper insights into factors influencing stock performance.

## Future Enhancements

To build upon this analysis, the following improvements are proposed:

- **Incorporate Dividend Analysis**: Evaluating dividend yields and payout ratios to assess the total return on investment.
- **Expand Dataset**: Including more financial institutions or extending the time frame for a more comprehensive analysis.
- **Predictive Modeling**: Implementing machine learning models to forecast future stock performance based on historical data.

For detailed analysis and visualizations, please refer to the [notebooks](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/tree/main/notebooks) and [dashboard](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/tree/main/dashboard) directories.

*Note: This project is for educational purposes only and does not constitute financial advice.*

