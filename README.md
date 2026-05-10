# Stock Price Analysis & News Sentiment Analysis

## Project Overview
This project analyzes stock price data and sentiment from news articles for major tech companies (AAPL, AMZN, GOOG, META, NVDA). It computes technical indicators and correlates them with news sentiment to identify trading signals and market trends.

## Features
- **Stock Price Data Loading**: Load historical price data for 5 major tickers
- **Technical Indicators**: 
  - Moving Averages (SMA, EMA)
  - Relative Strength Index (RSI)
  - MACD (Moving Average Convergence Divergence)
- **Data Validation**: Check for missing values and data quality
- **Visualization**: Charts and plots for technical analysis
- **Sentiment Analysis**: NLP-based sentiment extraction from news articles

## Project Structure
```
news-sentiment-analysis/
├── data/
│   ├── AAPL.csv
│   ├── AMZN.csv
│   ├── GOOG.csv
│   ├── META.csv
│   └── NVDA.csv
├── notebooks/
│   └── stock_price_analysis.ipynb
└── README.md
```

## Installation
```bash
pip install pandas numpy matplotlib seaborn nltk scikit-learn
```

## Usage
1. Open `notebooks/stock_price_analysis.ipynb`
2. Run cells in order:
   - Data Preparation
   - Moving Averages
   - RSI Calculation
   - MACD Calculation
3. View outputs and visualizations

## Technical Indicators

### Moving Averages (MA)
- **SMA_20/50**: Simple moving average over 20 and 50 periods
- **EMA_20/50**: Exponential moving average over 20 and 50 periods

### RSI (Relative Strength Index)
- Period: 14
- Overbought: > 70
- Oversold: < 30

### MACD
- Fast EMA: 12-period
- Slow EMA: 26-period
- Signal Line: 9-period EMA of MACD
- Histogram: MACD - Signal Line

## Data Sources
- Historical stock price CSV files located in `data/` folder
- Format: Date, Open, High, Low, Close, Volume

## Requirements
- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- nltk
- scikit-learn

## License
MIT

## Author
Ten Academy AI - Week 1