# JSC370 Final Project

## Project Website:
[https://justinzhaoovo.github.io/JSC370Final/](https://justinzhaoovo.github.io/JSC370Final/)

## Description

This project explores how a set of financial and macro indicators (implied volatility (VIX), the 10-year Treasury yield, gold prices, and the U.S. Dollar Index (DXY)) are associated with realized volatility of the S&P 500, using daily data from 2015 to 2025.

## Data

Data are collected from two sources:

- **FRED API** : VIX (VIXCLS), 10-year Treasury yield (DGS10)
- **Yahoo Finance** (`yfinance` package) : S&P 500 (^GSPC), Gold (GC=F), U.S. Dollar Index (DX-Y.NYB)

Raw data are cached locally in the `data/` folder.

## Setup

### 1. FRED API Key

Fetching data from FRED requires a free API key:

1. Register at [https://fredaccount.stlouisfed.org/login/secure/](https://fredaccount.stlouisfed.org/login/secure/)
2. After logging in, go to `API Keys` and request a key
3. Copy `.env.example` to `.env` and fill in your API key

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```