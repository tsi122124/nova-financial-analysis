# Nova Financial Analysis

This repository contains the Week 1 challenge project for the 10 Academy Artificial Intelligence Mastery Program. The project focuses on analyzing financial news sentiment and historical stock market data to understand how news sentiment may influence stock price movements.

---

# Project Objective

The goal of this project is to build a complete analytical pipeline that:

- Explores and analyzes financial news headlines
- Computes technical indicators from historical stock price data
- Applies sentiment analysis to financial news
- Measures the statistical relationship between news sentiment and stock price returns

The project is divided into three major tasks:

1. Exploratory Data Analysis (EDA)
2. Quantitative Financial Analysis using TA-Lib and PyNance
3. Correlation Analysis between News Sentiment and Stock Returns

---

# Repository Structure

```text
nova-financial-analysis/
│
├── .github/
│   └── workflows/
│       └── unittests.yml
│
├── data/
│   ├── newsData/
│   └── yfinance_data/
│
├── notebooks/
│   ├── task_1_eda.ipynb
│   └── task_2_quantitative_analysis.ipynb
│
├── scripts/
├── src/
├── tests/
│
├── requirements.txt
├── README.md
└── .gitignore
```

# Technologies and Libraries Used

## Data Analysis

- pandas
- numpy

## Visualization

- matplotlib
- seaborn

## NLP and Text Analysis

- scikit-learn
- nltk
- textblob
- vaderSentiment

## Financial Analysis

- TA-Lib
- PyNance
- yfinance

## Development Tools

- Git
- GitHub
- GitHub Actions
- Jupyter Notebook

# Environment Setup

## Clone Repository

git clone https://github.com/tsi122124/nova-financial-analysis.git

## Navigate into Project Directory

cd nova-financial-analysis

## Create Virtual Environment

### Windows

python -m venv venv
venv\Scripts\activate

### Linux / Mac

python3 -m venv venv
source venv/bin/activate

## Install Dependencies

pip install -r requirements.txt

# Running the Project

## Start Jupyter Notebook

jupyter notebook

Open notebooks from the `notebooks/` directory.

# CI/CD

GitHub Actions is configured through:

.github/workflows/unittests.yml

This workflow helps maintain repository quality and reproducibility.

# Dataset Notes

Large datasets are excluded from Git tracking using `.gitignore` because GitHub restricts files larger than 100MB.

Datasets should remain locally inside:

data/newsData/
data/yfinance_data/

# Tasks Completed

# Task 1 — Exploratory Data Analysis (EDA)

## Objectives

- Understand the structure and characteristics of the financial news dataset
- Analyze publishers, headline patterns, and publication trends
- Identify common financial keywords and topics

## Analysis Performed

### Data Loading and Cleaning

- Loaded financial news dataset
- Parsed datetime columns
- Verified missing values
- Engineered headline length feature

### Descriptive Statistics

- Headline length distribution
- Publisher activity analysis
- Publication frequency trends

### Text Analysis

- Keyword extraction using CountVectorizer
- Identification of common financial terms
- Topic exploration from headlines

### Time Series Analysis

- Publication trends over time
- Hourly publishing behavior analysis

### Publisher Analysis

- Most active publishers identified
- Distribution of article contributions explored

## Key Findings

- Financial headlines are concise and highly structured
- News publication spikes occur around market-relevant periods
- A small number of publishers dominate the dataset
- Frequent keywords are heavily related to earnings and analyst ratings

# Task 2 — Quantitative Financial Analysis

## Objectives

- Analyze historical Google stock price data
- Compute technical indicators using TA-Lib
- Visualize market trends and momentum indicators

## Data Preparation

- Loaded historical stock price data
- Converted dates into datetime format
- Verified data integrity
- Checked for missing values

## Technical Indicators Implemented

### Moving Averages

- Simple Moving Average (SMA 20, SMA 50)
- Exponential Moving Average (EMA 20)

### Momentum Indicators

- Relative Strength Index (RSI)
- Moving Average Convergence Divergence (MACD)

### Financial Metrics

- Daily returns
- Rolling volatility

## Visualizations

- Stock price with moving averages
- RSI indicator visualization
- MACD visualization

## Key Findings

- Google stock demonstrates long-term upward momentum
- RSI identifies periods of overbought and oversold conditions
- MACD captures momentum shifts and trend reversals
- Moving averages clearly smooth market trends

# Author

Tsion Habtesilasei
10 Academy — Artificial Intelligence Mastery Program

# License

This project is for educational and research purposes.
