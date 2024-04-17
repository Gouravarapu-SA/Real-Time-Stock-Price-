# Real-Time Stock Price Analysis Web Application

This document outlines a project to build an interactive real-time stock price dashboard web application using Python. The application fetches financial data, creates visualizations, compares stocks, and calculates portfolio returns. The project utilizes several Python libraries, including yfinance, ipyvuetify, cufflinks, and mercury.

## Introduction

The goal of this project is to analyze stock performance and portfolio management by fetching financial data, creating visualizations, and calculating portfolio returns. The application uses the following Python libraries:

- **yfinance**: Used to fetch financial data from Yahoo Finance.
- **ipyvuetify**: Helps create interactive web interfaces using Vuetify components.
- **cufflinks**: Simplifies data visualization with Plotly.
- **mercury**: Converts the Jupyter notebook into a web application.

## Setup

1. Install the required libraries (yfinance, ipyvuetify, cufflinks, and mercury) using pip.
2. Import the necessary libraries: pandas, cufflinks, numpy, yfinance, datetime, warnings, mercury, and relativedelta.

### Configure Mercury App

- Create an instance of the Mercury app by providing a title, description, and toggling code visibility.
- Define input widgets to allow users to select a stock ticker symbol and time period in months for analysis. The ticker widget provides a dropdown of semiconductor stocks (NVDA, INTC, AMD, TSM, MU), and the period widget is a numeric input ranging from 1 to 12 months.

## Visualize Stock Performance

- Use the selected ticker symbol and time period to download the stock data from Yahoo Finance using the yfinance library.
- Create various visualizations with cufflinks and Plotly to analyze the data:
  - Line plot of adjusted close prices
  - Filled area plot of adjusted close
  - Returns plot with a best fit line
- Create a QuantFig to add technical indicators like SMA, Bollinger Bands, and volume to gain further insights.
- Download multiple semiconductor stocks and visualize their adjusted close prices in a comparative line plot.

## Compare Semiconductor Stocks

- Download data for multiple semiconductor stocks.
- Visualize their adjusted close prices in a comparative line plot.

## Calculate Cumulative Returns

- Calculate daily returns from adjusted close prices.
- Define weights for a sample semiconductor portfolio.
- Calculate weighted returns and then derive cumulative returns for the portfolio.
- Visualize the cumulative returns.

This detailed report walks through the key steps and code involved in building the interactive stock analysis web application using Python libraries. The report summarizes the goals, tools, visualizations, and calculations to provide insights into stock performance and portfolio management.
