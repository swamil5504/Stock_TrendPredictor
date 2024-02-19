
# Stock Price Prediction using LSTM with Keras

This project is a Python script that uses Long Short-Term Memory (LSTM) models implemented with Keras to predict the trends of Apple Inc. (AAPL) stock prices. It fetches historical stock data using the yfinance library and trains an LSTM model on the data to make future price predictions.

## How to Run

To run this code and predict stock prices, follow these steps:

1. Open the code in a Jupyter Notebook or in Google Colab.
2. Install the necessary dependencies, such as numpy, pandas, matplotlib, pandas_datareader, and yfinance.
3. Set the desired date range for fetching historical stock data by modifying the `start` and `end` variables.
4. Run the code cell by cell to execute the different sections of the code.

## Important Details

- Stock Symbol: AAPL (Apple Inc.)
- Stock Exchange: NASDAQ

Please ensure that you have the correct stock symbol and exchange information before running the code. You can modify the code to fetch data for a different stock by changing the value of the 'symbol' parameter in the `yf.download()` function.

## Parameters and Variables

Here are some important parameters and variables that you may need to modify:

- `start` and `end`: The date range for fetching historical stock data.
- LSTM units: The number of LSTM units in each layer of the model.
- Scaling: The feature scaling range for the MinMaxScaler.

## Code Overview

The main sections of the code are as follows:

1. Data Retrieval: The code fetches historical stock data for AAPL using the yfinance library.
2. Data Preprocessing: The code preprocesses the data by removing unnecessary columns, normalizing the values using MinMaxScaler, and splitting it into training and testing datasets.
3. Model Training: The code defines and trains an LSTM model using the training data.
4. Prediction: The code makes predictions for future stock prices using the trained model and evaluates the results.
5. Visualization: The code plots the original and predicted stock prices using matplotlib.

## Additional Information

- The shape of the training and testing data is displayed in the code.
- The model is evaluated using the mean squared error loss.
- The predictions are scaled back to the original price range for better interpretation.
- The code saves the trained model as 'keras_model.h5'.

Please note that this is a simplified example and may not provide accurate predictions in real-world scenarios. Use it for educational purposes and experiment with different configurations and techniques to improve the results.
