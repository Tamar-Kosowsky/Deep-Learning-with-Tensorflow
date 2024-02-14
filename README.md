# Deep-Learning-with-Tensorflow

# Project Rhythmic File: Predicting SPY Historical Prices with RNN

## Project Overview:
This project focuses on utilizing Recurrent Neural Networks (RNN), specifically LSTM and GRU models, to predict historical prices of SPY (SPDR S&P 500 ETF Trust). The dataset "SPY.csv" is used for training and evaluation.

### Data Preparation:
- Data is read from 'SPY.csv' and preprocessed to handle missing values.
- The dataset is split into training and testing sets, normalized using MinMaxScaler, and sequenced for RNN training.

### Model Architecture:
- Two types of models, GRU and LSTM, are designed with 3 RNN layers each for time series forecasting.
- The models are compiled with 'adam' optimizer and 'mean_squared_error' loss function.

### Model Training:
- The models are trained using TimeseriesGenerator for training and validation data.
- Early stopping is implemented to prevent overfitting during training.

### Model Evaluation:
- The performance of the models is evaluated using Mean Squared Error (MSE) and Mean Absolute Error (MAE).
- Model predictions are generated and compared against actual SPY prices.

### Outcome:
- Both LSTM and GRU models exhibit similar and accurate results.
- Due to better performance, the GRU model is selected for further use.
- The trained GRU model is saved as 'gru_model.h5', and the MinMaxScaler is saved as 'gru_scalar.pkl'.

## Next Steps:
- Implement the GRU model for predicting future SPY prices.
- Develop a pipeline for predicting prices for the next week using the trained model.

---
### Note:
This project demonstrates the successful implementation of RNN models for time series forecasting of SPY historical prices. The thorough evaluation and selection of the GRU model ensure reliable predictions for future price trends. For any further inquiries or assistance, feel free to reach out.



