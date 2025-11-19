# Web3 Trading Analysis: Market Sentiment vs Trader Behavior

## 📊 Project Overview

This project analyzes the relationship between Bitcoin market sentiment (Fear & Greed Index) and actual trading behavior on the Hyperliquid exchange. The analysis reveals how trader profitability, risk patterns, volume, and trading decisions align or diverge from overall market sentiment.

## 🎯 Objective

Explore and analyze how trading behavior (profitability, risk, volume, leverage) aligns or diverges from overall market sentiment (fear vs greed). Identify hidden trends or signals that could influence smarter trading strategies.

## 📂 Project Structure

```
ds_Amir/
├── notebook_1.ipynb           # Complete analysis
├── csv_files/                 # Processed data and analysis outputs
│   ├── merged_trading_sentiment.csv
│   ├── volume_by_sentiment.csv
│   ├── pnl_by_sentiment.csv
│   ├── side_by_sentiment.csv
│   ├── daily_trading_patterns.csv
│   ├── correlation_matrix.csv
│   ├── summary_statistics.csv
│   ├── key_insights.txt
│   └── trading_recommendations.txt
|   |__ fear_greed_index.csv      # Bitcoin market sentiment dataset
|   |__ historical_data.csv       # Hyperliquid trading data
├── outputs/                      # Visualizations and charts
│   ├── sentiment_distribution.png
│   ├── volume_analysis.png
│   ├── profitability_analysis.png
│   ├── buy_sell_analysis.png
│   ├── top_coins_by_sentiment.png
│   ├── time_series_analysis.png
│   ├── correlation_heatmap.png
│   └── distribution_analysis.png
├── ds_report.pdf            
└── README.md               
```
 
 
 
## 📋 Datasets

### 1. Fear & Greed Index
- **Source**: Bitcoin market sentiment data
- **Columns**: `timestamp`, `value`, `classification`, `date`
- **Classification**: Extreme Fear, Fear, Neutral, Greed, Extreme Greed

### 2. Historical Trading Data (Hyperliquid)
- **Source**: Real trading data from Hyperliquid exchange
- **Key Columns**: 
  - `Account`: Trader wallet address
  - `Coin`: Cryptocurrency traded
  - `Execution Price`: Trade execution price
  - `Size Tokens`: Trade size in tokens
  - `Size USD`: Trade size in USD
  - `Side`: BUY or SELL
  - `Timestamp`: Trade timestamp
  - `Closed PnL`: Profit/Loss from closed positions
  - `Direction`: Trade direction

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.8+
pip install pandas numpy matplotlib seaborn jupyter
```

### Installation

1. Clone or download this project
2. Navigate to the project directory:
   ```bash
   cd ds_Amir
   ```

3. Install required packages:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

### Running the Analysis

#### Option 1: Google Colab
1. Upload `notebook_1.ipynb` to Google Colab
2. Upload `fear_greed_index.csv` and `historical_data.csv` to Colab
3. Run all cells sequentially

#### Option 2: Local Jupyter Notebook
```bash
jupyter notebook notebook_1.ipynb
```

## 📊 Analysis Components

### 1. Data Loading & Preprocessing
- Loading both datasets
- Date formatting and alignment
- Merging trading data with sentiment data
- Data cleaning and validation

### 2. Exploratory Data Analysis (EDA)
- **Sentiment Distribution**: Market sentiment patterns over time
- **Volume Analysis**: Trading volume by sentiment classification
- **Profitability Analysis**: PnL patterns across different sentiment periods
- **Buy/Sell Behavior**: Trading direction preferences by sentiment
- **Coin Analysis**: Most traded cryptocurrencies per sentiment
- **Time Series**: Daily trading patterns and trends
- **Correlation Analysis**: Relationships between sentiment and trading metrics
- **Distribution Analysis**: Statistical distributions of key metrics

### 3. Visualizations Generated
All visualizations are saved to the `outputs/` directory:
1. Sentiment distribution over time
2. Volume analysis by sentiment
3. Profitability metrics and win rates
4. Buy vs Sell behavior patterns
5. Top traded coins per sentiment
6. Time series analysis
7. Correlation heatmap
8. Distribution plots

### 4. Key Insights
The analysis reveals:
- Which market sentiment periods are most profitable
- Trading volume patterns during fear vs greed
- Win rate differences across sentiment classifications
- Optimal entry/exit timing based on sentiment shifts
- Coin performance variations by sentiment

### 5. Strategic Recommendations
- Sentiment-based entry/exit strategies
- Volume-based trading signals
- Risk management guidelines per sentiment
- Contrarian opportunity identification
- Asset allocation strategies

## 📈 Key Findings

Results are automatically generated in `csv_files/key_insights.txt` and include:
- Most active sentiment periods
- Most/least profitable sentiment classifications
- Highest win rates by sentiment
- Volume distribution patterns
- Correlation metrics
- Trader and coin statistics

## 🎓 Technical Details

### Libraries Used
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computations
- **matplotlib**: Data visualization
- **seaborn**: Statistical visualizations
- **datetime**: Date/time handling

### Analysis Techniques
- Groupby aggregations for sentiment-based analysis
- Time series analysis for trend identification
- Correlation analysis for relationship discovery
- Statistical summarization and distribution analysis
- Box plots for outlier detection
- Heatmaps for correlation visualization

## 📝 Output Files

### CSV Files (csv_files/)
- `merged_trading_sentiment.csv`: Combined dataset
- `volume_by_sentiment.csv`: Volume statistics by sentiment
- `pnl_by_sentiment.csv`: Profitability metrics by sentiment
- `side_by_sentiment.csv`: Buy/sell statistics
- `daily_trading_patterns.csv`: Daily aggregated metrics
- `correlation_matrix.csv`: Correlation coefficients
- `summary_statistics.csv`: Overall statistics
- `key_insights.txt`: Key findings text summary
- `trading_recommendations.txt`: Strategic recommendations

### Visualizations (outputs/)
All charts are saved as high-resolution PNG files (300 DPI)

## 🔍 How to Interpret Results

1. **Sentiment Value**: 0-100 scale (lower = fear, higher = greed)
2. **PnL Analysis**: Positive values = profit, negative = loss
3. **Win Rate**: Percentage of profitable trades
4. **Volume**: Trading activity measured in USD
5. **Correlation**: -1 to 1 (negative to positive relationship)

## 🎯 Next Steps

1. Review `notebook_1.ipynb` for complete analysis
2. Check `ds_report.pdf` for comprehensive insights
3. Explore visualizations in `outputs/` directory
4. Review data files in `csv_files/` for detailed metrics

