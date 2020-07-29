# Stock Market Data Analysis: Using Python to Visualize S&P500 Data in Tableau 
This program uses Python to get data from Yahoo Finance including daily pricing data (open, high, low, close, adj close, volume), market capitalization, and information about the companies (i.e. sector, industry, headquarters). 

## How to Run
* Use the "Stock_Market_Data_Analysis.ipynb" file to run the program in Jupyter Notebook. Use the .py file to run the program only in Python.
  * For users running the project with Jupyter:

1) After downloading the files, if Python is not installed, please install Python from https://www.python.org.
2) After installing Python, open a Python shell and run the following command:
   * "pip install pandas, pandas-datareader, beautifulsoup4, yfinance"
3) You will also need to install Jupyter Notebook, so from the shell run the command:
   * "pip install jupyter"
4) Once everything is installed, change directory (cd) to navigate to where the project has been downloaded. 
5) Locate the ".ipynb" file and run Jupyter with the command "jupyter notebook"; this will take you to the project in Jupyter Notebook, opening up a browser.
6) To view the project in Jupyter, select "Cell," and "Run All."

## Technical Summary
* Back end language: Python (the version used here is Python 3.7.6)
* Dataset: csv, stock price data via Yahoo Finance
* Packages: Pandas/NumPy for data manipulation.

## Features
The script will scrape data for S&P500 (i.e. ticker, security, sector), pull financial data from Yahoo Finance API, and download into a csv file to use as a data source in Tableau. It will also manipulate/clean data, and merge multiple data frames into one large csv file. The script uses for loops, dictionaries, and error handling. Additional features are highlighted below:
* Scrape stock tickers and company data from web (i.e. Wikipedia). 
* For this project, the SP500 list is from: "List of S&P 500 Companies" at https://en.wikipedia.org/wiki/List_of_S%26P_500_companies.
* Use Requests to scrape data for Beautiful Soup to parse.
* Using this soup object, navigate/search HTML for data you want to pull. 
* Create dictionary for all 500 companies, and pull daily stock price data over time (i.e. 01/01/2018 to now) and current market cap via Yahoo Finance. 

## Milestones
Import needed packages/modules
<b>Required for this project:</b>
* pandas
* pandas-datareader
* beautifulsoup4
* yfinance (or another finance API) 

## Requirements
* Build webscraper to get data for S&P500 List</b>
* Use Yahoo Finance (or other) API for financial data.
* Use Pandas to join stock tickers with financial data.
* Download data as csv and read. 
