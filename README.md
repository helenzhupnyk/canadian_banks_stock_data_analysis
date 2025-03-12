# Canadian Banks Stock Data Analysis

## Project Overview

**Authors:**  
- [Mariia-Olena Zhupnyk](https://github.com/helenzhupnyk)  
- [Mariia Shekhovtsova](https://github.com/Maria20892)

This project aims to analyze the stock performance of major Canadian banks over a specific period. By leveraging historical stock data, we seek to identify trends, assess market volatility, and provide data-driven insights to support informed investment decisions.  
For a detailed analysis, refer to the full report: [Canadian Banks Stock Report](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/blob/main/reports/Canadian_Banks_Stock_Report_draft1.pdf)

### Goals  
- Analyze historical stock price trends for major Canadian banks.  
- Assess market volatility and its impact on stock performance.  
- Identify correlations between stock price movements and external factors.  
- Develop predictive models to forecast future stock prices.  
- Present insights through interactive dashboards and reports.   

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

## Methodology

The analysis of Canadian bank stock data involves several key tools, techniques, and steps, outlined below:

### Tools:
- **Python**: The primary programming language used for data manipulation, analysis, and visualization.
- **Pandas**: Utilized for loading, cleaning, and transforming the data into DataFrames.
- **Matplotlib/Seaborn**: Used for data visualization to create graphs and charts that help in understanding stock trends.
- **Jupyter Notebook**: An interactive environment for running Python code, visualizing data, and documenting analysis.
- **Scikit-learn**: Applied for implementing machine learning algorithms like regression for predictive modeling.
- **Statsmodels**: Used for statistical analysis, including time-series forecasting models such as ARIMA.
- **Power BI**: For building interactive dashboards to visualize stock trends and analysis results.

### Techniques:
- **Data Cleaning**: Handling missing values, dropping irrelevant columns, and converting data types to prepare the dataset for analysis.
- **Exploratory Data Analysis (EDA)**: Examining the dataset through summary statistics and visualizations to identify patterns, trends, and correlations.
- **Moving Averages**: Calculating Simple Moving Averages (SMA) and Exponential Moving Averages (EMA) to identify trends and forecast stock price movements.
- **Volatility Analysis**: Measuring the variability in stock prices over time to assess market risk.
- **Correlation Analysis**: Analyzing the relationships between stock returns of different banks to identify potential diversification opportunities.
- **Time Series Forecasting**: Implementing ARIMA and other predictive models to forecast future stock prices based on historical data.
- **Monte Carlo Simulation**: A Monte Carlo Simulation is used to simulate a wide range of possible future stock price outcomes based on historical data and the distribution of returns.

### Steps:
1. **Data Collection**: Stock price data for Canadian banks is gathered from Yahoo Finance and stored in a PostgreSQL database.
2. **Data Cleaning & Preprocessing**: Data is loaded into a Pandas DataFrame, unnecessary columns are dropped, and the date column is converted into a DateTime format.
3. **Exploratory Data Analysis (EDA)**: Basic statistical analysis and visualizations are performed to understand the data and its patterns.
4. **Feature Engineering**: New features such as moving averages and returns are created to enhance the predictive models.
5. **Model Building**: Time series forecasting models (e.g., ARIMA) are trained and tested on the dataset to predict future stock prices.
6. **Evaluation & Recommendations**: The models are evaluated for accuracy, and investment recommendations are provided based on the analysis results.

This methodology allows us to gain insights into stock performance, predict future trends, and make data-driven investment decisions.

## Findings & Insights  

Our analysis of Canadian bank stocks provides valuable insights into their performance, volatility, and predictive trends. The key findings are based on **exploratory data analysis (EDA)**, **Monte Carlo simulations**, **ARIMA forecasting**, and interactive **dashboard visualizations**.  

### 1. Stock Performance Trends  
- All five banks—**BMO, BNS, CM, RY, and TD**—demonstrated **steady growth** over the analyzed period.  
- **RBC (RY) and TD Bank (TD)** showed the most consistent upward trends, making them relatively stable investments.  

### 2. Volatility Assessment  
- While all banks experienced **periods of volatility**, **CIBC (CM)** exhibited the highest fluctuations, suggesting higher risk but potential for short-term gains.  
- **BMO and RBC stocks** showed more resilience to market shocks, making them suitable for risk-averse investors.  
- **Monte Carlo simulations** highlighted the range of possible future stock prices, emphasizing the uncertainty in short-term predictions.  

### 3. Correlation Analysis  
- A **strong positive correlation** was observed between the stock prices of all five banks.  
- This suggests that external macroeconomic factors—such as **interest rates, inflation, and financial sector performance**—affect all banks similarly.  
- **Diversification within Canadian bank stocks may not significantly reduce risk** since they move in tandem.  

### 4. Predictive Modeling & Forecasting  
- **ARIMA models** provided reasonable short-term predictions, with RBC and TD showing the **most predictable trends**.  
- **Monte Carlo simulations** demonstrated a range of possible future prices, helping assess potential risks.  
- Future stock performance is **highly dependent on economic conditions**, making continuous monitoring essential.  

### 5. Interactive Dashboard Insights  
- Our **Power BI dashboard** presents real-time trends, moving averages, and volatility indicators for each bank.  
- Users can filter by **date range, stock ticker, and performance metrics** to gain personalized insights.  
- A comparison of **historical vs. predicted prices** helps assess model accuracy and investment potential.

![image](https://github.com/user-attachments/assets/82ef8f55-fe2a-4d60-a0b4-73b245522047)
![image](https://github.com/user-attachments/assets/e595c902-46ae-447c-817c-4ba715a25175)

**Explore our interactive dashboard:** [Stock Analysis Dashboard](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/tree/main/dashboard)  

For a deeper dive into the analysis, check out our notebooks:  
- [Exploratory Data Analysis (EDA)](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/blob/main/notebooks/02_EDA.ipynb)  
- [Monte Carlo Simulation & Predictions](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/blob/main/notebooks/03_Predictions_Visualization_Monte_Carlo_Simulation.ipynb)  
- [Advanced Data Analysis](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/blob/mariia/data_analysis.ipynb)  
- [ARIMA Forecasting](https://github.com/helenzhupnyk/canadian_banks_stock_data_analysis/blob/mariia/ARIMA_prediction.ipynb)  

These findings provide **actionable insights** for investors, helping them assess risk, identify trends, and make informed investment decisions. 🚀  

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

