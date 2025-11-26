Price and Trend Prediction(LSTM, TRANFORMER|OHLCV|PRICE AND TREND)

Feature Engineering and Selection(Boruta Algorithm, Recursive Feature Elimination , Hierarchical Clustering|NaN|FEATURES)

Volatility Prediction(GARCH, EGARCH, Hybrid LSTM, TCN (Temporal Convolutional Networks)|SQUARED RETURNS|VOLATILITY)

Adaptive Strategy and Ensemble Models
Risk and Position Management

Funding Rate Divergence
Open Interest (OI) vs. Volume Ratio
Liquidation Clusters
Regime Detection Features
GARCH Variants (Statistical Approach)
Deep Learning Volatility Models
Realized Volatility (RV) Estimators
Boruta Algorithm
Recursive Feature Elimination (RFE)
Hierarchical Clustering

Architectural Blueprint for Automation
A complete "Volatility-Gated" Architecture looks like this:

Data Ingestion: WebSocket streams (L2 Book, Trades, Funding).

Feature Store: Real-time calculation of OI Delta, Funding Divergence, and CVD.

Regime Classifier (HMM): Decides "Are we in a Trend or Chop?"

Volatility Predictor (LSTM): Predicts "How big will the next move be?"

Execution Engine:

If Regime = Trend & Volatility = High: Aggressive Entry (Market Orders).

If Regime = Chop & Volatility = Low: Passive Market Making (Limit Orders).


https://gemini.google.com/share/e8b5f262a9c5
