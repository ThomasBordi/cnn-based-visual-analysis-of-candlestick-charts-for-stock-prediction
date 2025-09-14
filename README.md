# Deep Learning for Candlestick Chart Classification  
**Predicting Stock Price Movements Using Convolutional Neural Networks**

## Summary
This work investigates the use of deep learning for predicting stock price movements from candlestick chart images. Both Convolutional Neural Networks (CNNs) and Long Short-Term Memory (LSTM) networks were evaluated on minute-level OHLCV data across multiple time intervals (1-, 5-, and 15-minute) and chart types (traditional candlestick, Heiken Ashi, and pattern-enhanced with indicators such as bullish engulfing and Doji).

Key findings include:
- CNNs perform well for basic candlestick pattern recognition, particularly with 5-minute intervals.  
- LSTM models outperform CNNs by capturing temporal dependencies in chart sequences.  
- The best result, **63.9% validation accuracy**, was achieved with an LSTM model trained on 8-day sequences with augmented chart types.  

These results suggest that LSTMs are more effective than CNNs for capturing both visual and temporal aspects of financial time-series data.


## Citation
@misc{bordino2025candlestick,
title={Deep Learning for Candlestick Chart Classification: Predicting Stock Price Movements Using Convolutional Neural Networks},
author={Thomas Bordino},
year={2025},
institution={Columbia University}
}
