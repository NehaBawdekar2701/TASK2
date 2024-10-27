# TASK2
Overview
The goal of this project is to create a machine learning-based trading strategy by predicting price movements based on engineered features from OHLC data. The project follows these main steps:

Feature Engineering: Create a diverse set of features from OHLC data.
Data Preprocessing: Normalize and standardize the features.
Model Development: Train a model to predict price movements and generate trading signals.
Backtesting and Performance Metrics: Evaluate strategy performance.
Validation and Out-of-Sample Testing: Check for generalizability of the model on unseen data.
Features
Technical Indicators: Moving Averages, RSI, MACD, Bollinger Bands, etc.
Price Action Features: High-low spreads, momentum, volatility.
Statistical Features: Rolling means, variances, skewness, kurtosis.
Lagged Features: Lagged values of prices, volume, and indicators.
Install Dependencies:

Install required packages from requirements.txt.
Optional: Create a virtual environment.
Data Preparation: Ensure the OHLC dataset is in CSV format with columns such as Date, Open, High, Low, Close, and Volume. Place the dataset in the data/ directory.
Step-by-Step Workflow
1. Feature Engineering
Objective: Generate a set of features that add predictive value to raw OHLC data.
Process: Compute technical indicators, price action features, rolling statistics, and lagged features to capture various market aspects.
2. Data Preprocessing: Normalization and Standardization
Objective: Scale features so they share a similar range, facilitating model training.
Process: Normalize and standardize features to ensure consistency across different types of data, improving model interpretability and performance.
3. Model Development and Training
Objective: Train a machine learning model to generate trading signals based on engineered features.
Process: Define the target variable (e.g., future price movement) and split the data into training and validation sets. Train a suitable machine learning model such as Random Forest or Gradient Boosting, and evaluate its predictive accuracy.
4. Backtesting and Performance Metrics
Objective: Simulate trades based on model predictions and assess performance.
Process: Use a backtesting framework to evaluate how the model’s predictions would perform in a trading scenario. Calculate metrics like Sharpe Ratio, Max Drawdown, Accuracy, Precision, Recall, and Cumulative Returns to gauge effectiveness.
5. Validation and Out-of-Sample Testing
Objective: Confirm that the model generalizes well on unseen data to avoid overfitting.
Process: Apply the trained model on out-of-sample data and compare performance metrics from both in-sample and out-of-sample testing to assess generalizability.
6. Strategy Development
Objective: Finalize a trading strategy based on model predictions, with clear entry/exit rules, risk management, and position sizing.
Process: Define decision rules for executing trades based on model output. Incorporate risk management principles to limit potential losses.
Results
The project evaluates the performance of the machine learning-based trading strategy with the following key metrics:

Sharpe Ratio: Measures risk-adjusted returns.
Max Drawdown: Indicates maximum observed loss from peak to trough.
Accuracy: Assesses how frequently the model predicts correctly.
Precision and Recall: For classification models, shows relevance and completeness of the predictions.
Cumulative Returns: Measures total returns over the testing period.
Sample results include visualizations of equity curves, drawdown charts, and cumulative returns, along with performance comparisons across training, validation, and out-of-sample datasets.
