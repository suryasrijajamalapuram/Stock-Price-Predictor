# Stock Price Prediction using LSTM

## Project Overview
This project predicts daily stock prices using a Long Short-Term Memory (LSTM) neural network. 
Using five years of historical stock data, the model captures trends and patterns to forecast next-day prices.

## Dataset
- Historical stock data containing Open, High, Low, Close, Volume, and Adjusted Close prices.
- The 'Close' price was used as the target for prediction.
- Data sourced from Kaggle: Time Series Forecasting with Yahoo Stock Price dataset.

## Approach
1. **Data Preprocessing**
   - Extracted the 'Close' price.
   - Scaled values between 0 and 1 using MinMaxScaler.
   - Created sequences of 60 consecutive days to predict the next day.

2. **Model Development**
   - Built a 2-layer LSTM model with 50 units per layer and dropout for regularization.
   - Trained the model for 20 epochs with batch size 32.
   - Loss function: Mean Squared Error (MSE), Optimizer: Adam.

3. **Evaluation**
   - Predicted prices on the last 200 days of data.
   - Calculated metrics:
     - RMSE: 119.47
     - MAE: 107.84
     - R² Score: 0.624
   - Visualized predicted vs actual prices to assess model performance.

## Key Highlights
- Demonstrated ability to preprocess and sequence time-series data for neural network modeling.
- Developed an LSTM model capturing market trends with measurable predictive performance.
- Visualized results clearly, making trends interpretable and insights actionable.

## Libraries Used
- Python 3.x
- pandas, numpy, matplotlib
- scikit-learn
- tensorflow / keras

## Visualization
- Actual vs Predicted stock price plot for the test period:
---

This project highlights skills in **data preprocessing, time-series modeling, LSTM networks, evaluation, and visualization**, making it portfolio-ready and resume-appropriate.
