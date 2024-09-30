
# AI-Powered Trading Bot

This project implements an AI-powered trading bot that uses supervised machine learning to predict cryptocurrency price movements based on historical data. It leverages the Binance API to fetch trading data and trains a Random Forest model to make trading decisions.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This bot automates cryptocurrency trading by predicting the direction of price movement using a machine learning model. The goal is to execute trades based on these predictions, allowing for more efficient and data-driven trading strategies.

## Features

- Fetches historical price data using Binance API.
- Calculates technical indicators like moving averages and Relative Strength Index (RSI).
- Trains a Random Forest model to predict future price movements.
- Backtests the strategy to evaluate its effectiveness based on historical data.

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/your-private-repo.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd AI_Trading_Bot
   ```

3. **Install dependencies**:

   Install the required packages from the `requirements.txt` file:

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up Binance API keys**:

   Replace `your_api_key` and `your_api_secret` in the script with your actual Binance API key and secret. You can generate these from the Binance dashboard.

## Usage

1. **Running the bot**:

   To run the bot, execute the following script in a Jupyter Notebook or Python environment:

   ```python
   python trading_bot.py
   ```

   The bot will fetch historical data, train the model, and perform backtesting to simulate trading results.

2. **Backtesting**:

   You can run backtesting to evaluate the bot's performance based on historical data. The backtesting results will show cumulative returns based on the strategy applied.

3. **Customizing**:

   - You can modify the `SYMBOL` in the script to change the cryptocurrency pair (e.g., BTCUSDT, ETHUSDT).
   - You can also extend the feature set by adding additional technical indicators for better prediction performance.

## File Structure

```
.
├── src/
│   ├── trading_bot.py        # Main script for the AI-powered trading bot
│   ├── utils.py              # Utility functions (data fetching, feature engineering)
│   └── requirements.txt      # Python package dependencies
├── dataset/                  # Directory for dataset storage (if required)
├── examples/                 # Example usage of the trading bot
├── README.md                 # This README file
└── Dockerfile                # Dockerfile for containerization (optional)
```

## Requirements

- Python 3.x
- `python-binance`
- `pandas`
- `scikit-learn`
- `numpy`
- `ccxt`

Install the necessary Python packages using:

```bash
pip install -r requirements.txt
```

## Contributing

If you would like to contribute to this project, feel free to open a pull request or submit an issue. Contributions are welcome to improve the model, add more features, or optimize the bot’s performance.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
