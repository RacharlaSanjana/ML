## README

### Leveraging Momentum Effect in Machine Learning-based Cryptocurrency Trading

#### Introduction
This repository contains code and data for implementing a machine learning-based approach to cryptocurrency trading, focusing on leveraging the momentum effect. The momentum effect refers to the tendency of assets to persist in their performance trends over time. Traditional trading models often struggle to adapt to the volatile nature of cryptocurrency markets, making machine learning an appealing alternative for market forecasting and analysis.

#### Paper Summary
The associated paper explores the application of machine learning techniques in cryptocurrency trading, particularly targeting the momentum effect. It proposes a novel approach that combines market forecasting with supervised momentum analysis. By utilizing machine learning algorithms, the system aims to predict the likelihood and direction of momentum in cryptocurrency prices for the next trading day. The paper showcases promising results through backtesting on popular cryptocurrencies, demonstrating superior performance compared to heuristic approaches in terms of classification accuracy and return on investment.

#### Dataset
The dataset used in this study consists of historical cryptocurrency price data sourced from Kaggle. Specifically, CSV files for Bitcoin (BTC), Ethereum (ETH), and Litecoin (LTC) from the year 2020 are utilized. Each dataset initially contains 10,000 data points. Technical indicators such as Simple Moving Averages (SMA), Exponential Moving Averages (EMA), Moving Average Convergence Divergence (MACD), Relative Strength Index (RSI), Average True Range (ATR), and On-Balance Volume (OBV) are computed for each cryptocurrency.

#### Code Structure
1. **Data Acquisition and Preparation**: Import historical cryptocurrency price data from CSV files.
2. **Dataset Labeling**: Apply an indicator function to label each dataset sample as positive overreaction, negative overreaction, or normal day.
3. **Feature Design for ML Models**: Generate various technical indicators as features for machine learning models.
4. **Classification**: Utilize machine learning algorithms to classify dataset samples into different categories based on labeled data.
5. **Classification Results**: Report classification performance metrics, including the weighted F1 measure.

#### Exploratory Data Analysis (EDA) Insights
- The dataset comprises 9981 entries and 23 columns.
- Columns include features like Unix timestamp, open, high, low, close prices, volume, technical indicators, labels, price changes, moving averages, standard deviation, upper and lower bands, and volume rate of change.
- Missing values are present in some columns, particularly in MACD, RSI, OBV, Price_Diff, MA20, 20dSTD, UpperBand, LowerBand, and Volume_ROC.

#### Model Evaluation Results (BTC Data)
- Random Forest and Support Vector Classification (SVC) achieved the highest accuracy and precision scores, indicating relatively good performance in classifying the data.
- Random Forest, SVC, and K-Nearest Neighbors (KNN) exhibited the highest recall scores.
- Multi-Layer Perceptron (MLP) also showed promising performance across accuracy, precision, and recall metrics.
- Gaussian Naive Bayes (GNB) and Heuristic Function (HE) demonstrated lower performance compared to other models.

#### Conclusion
Based on the evaluation metrics, Random Forest, SVC, and KNN appear to be the most promising models for the classification task. These models could potentially offer effective solutions for managing excessive price volatility in cryptocurrency trading, thereby improving trading outcomes for investors navigating dynamic markets.

