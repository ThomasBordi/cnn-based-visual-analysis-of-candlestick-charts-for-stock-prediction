# Deep Learning for Candlestick Chart Classification

## Predicting Stock Price Movements Using Convolutional Neural Networks

**Author:** Thomas Bordino (Columbia University)

### Abstract

This research explores the effectiveness of deep learning models, particularly Convolutional Neural Networks (CNNs) and Long Short-Term Memory (LSTM) networks, for predicting stock price movements based on candlestick chart data. The study aims to predict the trend of the last hour of a trading day using OHLCV data from current and previous trading days.

**Key Achievement:** Best validation accuracy of 63.9% with LSTM model using 8-day sequences.

---

## 📊 Research Overview

### Problem Statement
- **Objective:** Predict stock price trend for the last hour of trading day
- **Input:** Candlestick charts from current and previous days
- **Output:** Binary classification (up/down trend)

---

## 🔑 Key Insights

### What Works Best
- **LSTM models beat CNNs** for time series prediction (63.9% vs ~56% accuracy)
- **5-minute intervals** provide optimal balance between detail and noise
- **Heiken Ashi charts** with pattern highlighting improve performance by ~4%
- **8-day sequences** are the sweet spot for temporal modeling

### Surprising Findings
- Pre-trained ResNet performed poorly (53%) - financial charts differ too much from natural images
- Multi-interval inputs didn't help - single 5-minute interval was sufficient
- Attention mechanisms provided minimal benefit
- Simple architectures often outperform complex ones for individual charts

---

## 💡 Practical Takeaways

1. **LSTMs are worth the complexity** for sequential financial data
2. **Chart augmentations matter** - Heiken Ashi + pattern highlighting beats vanilla candlesticks
3. **5-minute resolution** hits the sweet spot for intraday patterns

---

## Dataset
24 tickers, 2000-2024, 3+ million charts via Alpha Vantage API
