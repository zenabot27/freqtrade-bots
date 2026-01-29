# Crypto Trading Bots

Automated cryptocurrency trading strategies using [Freqtrade](https://www.freqtrade.io/).

## Strategies

### 1. GodStra
- **Author**: @Mablue (Masoud Azizi)
- **Logic**: Multi-indicator strategy using 60+ TA features with genetic algorithm optimization
- **Timeframe**: 12h
- **ROI**: 35.56% at 0h, decreasing to 0% after 15 days
- **Stoploss**: -34.5%

### 2. PatternRecognition
- **Author**: @Mablue
- **Logic**: K-line pattern recognition using TA-Lib (e.g., CDLHIGHWAVE)
- **Timeframe**: 1d
- **ROI**: 93.6% at 0h, decreasing to 0% after 33 days
- **Stoploss**: -28.8%

### 3. SuperTrend
- **Author**: @juankysoriano
- **Logic**: Triple SuperTrend trend confirmation (all 3 indicators must show "up")
- **Timeframe**: 1h
- **ROI**: 8.7% at 0h, decreasing to 0% after 37 hours
- **Stoploss**: -26.5%

## Quick Start

```bash
# Clone the repo
git clone https://github.com/qq-agent-hao/crypto-bots.git
cd crypto-bots

# Install dependencies
pip install -r requirements.txt

# Run a bot
freqtrade trade --config user_data/config_godstra.json --strategy GodStra
```

## Configuration

Each strategy has its own config file in `user_data/`:
- `config_godstra.json` - GodStra strategy
- `config_pattern.json` - PatternRecognition strategy
- `config_supertrend.json` - SuperTrend strategy

## Disclaimer

⚠️ **Trading cryptocurrencies carries high risk. Please only invest what you can afford to lose.** This software is for educational purposes only. The author is not responsible for any financial losses.

## License

MIT
