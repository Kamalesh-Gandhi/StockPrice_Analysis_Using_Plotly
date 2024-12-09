# Stock Analysis Project

## Overview
This project performs a detailed analysis of stock data, focusing on stocks listed on the National Stock Exchange of India (NSE). The analysis includes visualization of stock prices, specifically focusing on the closing prices, and creating interactive animations to visualize how these stock prices change over time.

The stocks analyzed in this project are:
- **ITC**
- **TCS**
- **LTTS**
- **ABCAPITAL**
- **HDFCBANK**

## Description
This project provides an in-depth analysis and visualization of historical stock price data from the National Stock Exchange of India (NSE). The goal is to understand how the closing prices of selected stocks evolve over time and provide insights into their price trends.

### Key Features:
1. **Stock Selection**: The project analyzes data for the following stocks:
   - **ITC**: ITC Limited, a leading FMCG company.
   - **TCS**: Tata Consultancy Services, one of India's largest IT services companies.
   - **LTTS**: L&T Technology Services, a provider of engineering and technology solutions.
   - **ABCAPITAL**: Aditya Birla Capital, a financial services company.
   - **HDFCBANK**: HDFC Bank, one of India's leading private sector banks.

2. **Data Extraction and Transformation**: 
   The raw stock data contains daily stock prices, including:
   - **Open, High, Low, Close, Volume**: These are the core data points used to understand the performance of a stock over time.
   - The project processes the `Date` column, extracting year, month, day, and week information for easier time-based analysis.

3. **Visualization**: 
   The primary feature of the project is the interactive **animated bar chart** created using Plotly. This chart displays:
   - **X-axis**: The names of the stocks (`Stock_Name`).
   - **Y-axis**: The closing prices (`Close`).
   - **Animation**: The bar chart animates across time (`Date`), showing how the closing prices change over different periods.
   - **Hover Data**: Additional information about each stock's daily performance such as opening price, highest and lowest price of the day, volume, and date-based details (day, month).
   - **Color Coding**: Each stock is uniquely color-coded to differentiate them in the visualization.

4. **Analysis and Insights**: 
   By visualizing the closing prices over time, the project aims to:
   - Identify trends and patterns in stock performance.
   - Compare the performance of multiple stocks simultaneously.
   - Explore the relationship between trading volume, price movement, and volatility.

5. **Interactivity**:
   - The animated chart allows users to explore how each stock's price evolves across different timeframes.
   - The hover feature provides detailed insights into daily price movements, aiding in further analysis.


## Project Workflow

### Data Loading & Preparation:
- The data is loaded into a pandas DataFrame (`Combined_StockData`), and additional columns for year, month, day, and week are derived from the `Date` column.

### Data Transformation:
- A `year_month` column is created by combining the `year` and `month` columns for easier time-based grouping.

### Data Visualization:
- An animated bar chart is created using Plotly Express, which visualizes the stock's closing prices over time (`Date`).
- The `animation_frame` is set to `Date` to show how the stock prices change for each stock over time.
- The bar chart includes hover data like `Close`, `High`, `Low`, `Open`, `Volume`, `day`, and `month`.


## Conclusion

This project allows for a comprehensive visualization of stock price trends over time. The animation provides insight into the fluctuations in stock prices, and the interactive nature of the Plotly visualizations allows for a dynamic exploration of the data. By analyzing these trends, users can better understand the historical performance of stocks and make more informed decisions in financial analysis.


## Installation

### Prerequisites
Ensure that you have the following libraries installed:

- **pandas**: For data manipulation and handling.
- **numpy**: For numerical operations.
- **plotly**: For interactive data visualization and animations.
- **matplotlib**: For static visualizations.

To install the necessary libraries, you can use the following commands:

```bash
pip install pandas numpy plotly matplotlib



