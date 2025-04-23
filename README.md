# Economic Data Processor & Vegetable Price Forecasting

This project combines the gathering, processing, and analysis of various economic data sources with forecasting vegetable prices using macroeconomic indicators. It integrates time series models such as VAR, VECM, and ARDL with economic data like fuel prices, exchange rates, inflation indices, and other commodity prices to predict future trends in vegetable prices.

## Project Overview

The project consists of two main parts:

1. **Economic Data Processor**: 
   - Scrapes and processes economic data from various online sources (like fuel prices, exchange rates, inflation indices, etc.).
   - Merges and cleans the data into a unified dataset for analysis and forecasting.

2. **Vegetable Price Forecasting**: 
   - Uses the processed economic data to forecast vegetable prices.
   - Employs advanced time series models such as Vector Autoregression (VAR), Vector Error Correction Model (VECM), and Autoregressive Distributed Lag (ARDL) to capture the relationships between macroeconomic indicators and vegetable price fluctuations.

## Key Features

- **Web Scraping**: Extracts data from government websites such as the CBSL for inflation, exchange rates, and price reports, and from CEYPETCO for fuel prices.
- **PDF Parsing**: Downloads and extracts data from PDF reports using OCR and text extraction.
- **Data Merging**: Combines data from multiple sources, including fuel prices, exchange rates, CCPI (inflation), and more, into a single dataset.
- **Data Cleaning**: Handles missing values, inconsistent formats, and aligns data across different sources to ensure uniformity.
- **Forecasting Models**: 
  - **VAR**: Models interdependencies among multiple time series.
  - **VECM**: Captures short-term adjustments and long-term equilibrium relationships when cointegration exists.
  - **ARDL**: Models the relationship between variables by considering both short-term and long-term dynamics.
- **Principal Component Analysis (PCA)**: Reduces dimensionality and improves model efficiency by identifying key components that drive the variations in economic data.

## Data Sources

The project pulls data from multiple sources, including:
- **Fuel Prices**: Historical data from CEYPETCO.
- **Exchange Rates**: Daily exchange rates from CBSL.
- **Inflation (CCPI)**: Consumer Price Index (CCPI) data from CBSL.
- **Price Reports**: Daily price reports from CBSL.

## Requirements

The following libraries are required to run the project:

- `requests`
- `pandas`
- `fitz` (PyMuPDF)
- `selenium`
- `pytesseract` (for OCR)
- `pdf2image` (to convert PDF to images)
- `statsmodels` (for time series models)
- `scikit-learn` (for PCA)

Install them using `pip`:

```bash
pip install requests pandas fitz selenium pytesseract pdf2image statsmodels scikit-learn
