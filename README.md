# Machine-Learning-for-Trading-Signal-Evaluation-FIXED-
Machine Learning–based trading signal evaluation using walk-forward backtesting to compare logistic regression and random forest models against traditional momentum and buy-and-hold strategies.

Project 5: Machine Learning for Trading Signal Evaluation

This project develops and evaluates machine learning–based trading signals using historical equity market data, with a strong focus on out-of-sample robustness, realistic execution assumptions, and proper backtesting methodology.

The workflow begins with downloading adjusted price data for a major equity ETF and constructing feature sets using only information available at time t, avoiding look-ahead bias. Features include short- and medium-term returns, momentum indicators, rolling volatility measures, trend signals based on moving averages, and RSI.

Two supervised learning models are implemented:

Logistic Regression (with standardized inputs)

Random Forest Classifier

Models are trained and evaluated using a rolling walk-forward framework, where fixed-length training windows are followed by forward testing periods. Model outputs are converted into long/flat trading signals using probability thresholds, and transaction costs are explicitly incorporated.

The strategies are benchmarked against:

Buy-and-Hold

A traditional 21-day momentum strategy

Performance is evaluated using both classification metrics (accuracy, precision, recall, F1, ROC-AUC) and trading metrics (annualized return, volatility, Sharpe ratio, maximum drawdown, and win rate). Results are visualized through equity curves and drawdown analysis, and all outputs are saved for reproducibility.

This project demonstrates a production-style quantitative research pipeline, combining financial intuition, machine learning, and disciplined backtesting practices.
