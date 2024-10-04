# DRL Ensemble Stock Trading

This project demonstrates a Deep Reinforcement Learning (DRL) ensemble approach for stock trading using multiple models: A2C, DDPG, PPO, SAC, and TD3. It uses the FinRL library to create a stock trading environment, download data, preprocess it, and apply technical indicators. The models are trained and then combined using weighted ensemble predictions to maximize profitability in the stock market.

## Features

- **Stock trading environment**: Simulates the stock market using Yahoo finance data.
- **Ensemble of DRL models**: Combines A2C, DDPG, PPO, TD3, and SAC models to make trading decisions.
- **Technical indicators**: Uses indicators like MACD, Bollinger Bands, RSI, CCI, and more for trading.
- **Performance Metrics**: Calculates Sharpe Ratio, Beta, Alpha, Sortino Ratio, and Volatility over a rolling window.

## Files

- **`DRL_Ensemble_Prediction_Stock_Trading.ipynb`**: The main notebook that sets up the stock trading environment, trains models, and uses ensemble predictions for stock trading.
- **`ensemble_stock_trading_metrics_analysis.py.ipynb`**: Notebook for calculating and visualizing performance metrics such as Sharpe Ratio, Alpha, Beta, Sortino Ratio, and Volatility.

## Installation

### 1. Clone the Repository
```bash
git clone <repository_url>
cd <repository_folder>
```

### 2. Install Required Libraries
You can install the necessary Python packages by running the following command:
```bash
pip install -r requirements.txt
```

### 3. Data Preparation
Ensure that you have the `trade_data.csv` file in your project directory for loading historical stock data.

### 4. Run the Code
You can execute the Jupyter notebooks or Python files in the environment of your choice, such as Jupyter Notebook, JupyterLab, or Visual Studio Code with Python support.

### 5. Model and Data
The model files are expected to be located in the directory defined by `TRAINED_MODEL_DIR`. You can use pretrained models or train new models using the provided code.

## Usage

1. Load the stock data using the `YahooDownloader`.
2. Split the data into training and trading sets.
3. Add technical indicators using the `ta` library.
4. Initialize the stock trading environment.
5. Load pretrained models (A2C, DDPG, PPO, SAC, TD3).
6. Use the ensemble prediction function to combine actions from different models and make trading decisions.
7. Analyze performance using performance metrics and visualize the results.

## Requirements

See `requirements.txt` for a list of all required dependencies.

### License

This project is licensed under the MIT License.
