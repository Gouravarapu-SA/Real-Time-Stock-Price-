# Real-Time-Stock-Price-
An interactive web application for real-time stock price analysis, including fetching financial data, creating visualizations, comparing stocks, and calculating portfolio returns
Introduction
The document outlines a project to build an interactive real-time stock price dashboard web application using Python. The goal is to analyze stock performance and portfolio management by fetching financial data, creating visualizations, and calculating portfolio returns.
The project uses several Python libraries including yfinance, ipyvuetify, cufflinks, and mercury. yfinance is used to fetch financial data from Yahoo Finance. ipyvuetify helps create interactive web interfaces using Vuetify components. cufflinks simplifies data visualization with Plotly. mercury converts the Jupyter notebook into a web application.
•
The first step is to install the required libraries yfinance, ipyvuetify, cufflinks, and mercury using pip.
•
The libraries are then imported: pandas, cufflinks, numpy, yfinance, datetime, warnings, mercury, and relativedelta.
Setup
Configure Mercury App
•
An instance of the Mercury app is created by providing a title, description, and toggling code visibility.
•
Input widgets are defined to let users select a stock ticker symbol and time period in months for analysis. The ticker widget provides a dropdown of semiconductor stocks (NVDA, INTC, AMD, TSM, MU). The period widget is a numeric input from 1 to 12 months.
Visualize Stock Performance
•
The selected ticker symbol and time period are used to download the stock data from Yahoo Finance using the yfinance library.
•
Various visualizations are created with cufflinks and plotly to analyze the data - line plot of adjusted close prices, filled area plot of adjusted close, returns plot with best fit line.
•
A QuantFig is created to add technical indicators like SMA, Bollinger Bands, volume to gain further insights.
Multiple semiconductor stocks are downloaded, and their adjusted close prices are visualized in a comparative line plot.
Calculate Cumulative Returns
Daily returns are calculated from adjusted close prices. Weights are defined for a sample semiconductor portfolio. Weighted returns are calculated and then cumulative returns for the portfolio are derived and visualized.
This detailed report walks through the key steps and code involved in building the interactive stock analysis web application using Python libraries. The report summarizes the goals, tools, visualizations, and calculations to provide insights into stock performance and portfolio management.
Compare Semiconductor Stocks
