# stock-price-prediction-and-comparison

This project focuses on predicting stock prices using machine learning models. The primary goal is to analyze stock price data, clean the dataset, and compare different models for stock price prediction.
## Project Structure

    untitled_7.ipynb: This Jupyter Notebook contains the code for data analysis, model training, and predictions.
    stock prices.csv: The dataset used for stock price predictions. It contains historical stock price data.

## Project Overview
Steps Involved:

    Data Loading:
        Loaded the stock prices.csv file, which contains stock price data for multiple stocks.

    Data Preprocessing:
        Removed null values and handled outliers to clean the dataset for better model performance.

    Single Stock Prediction with LSTM:
        Trained an LSTM (Long Short-Term Memory) model for a single stock.
        Achieved a Mean Absolute Error (MAE) of 0.02.

    Comparison with Prophet:
        Used the Prophet model for the same stock prediction task.
        Achieved an MAE of 16.2 (higher error than LSTM).
        LSTM performed better in this case, as lower MAE is preferred.

    Multi-Stock Prediction with LSTM:
        Trained the LSTM model for multiple stocks simultaneously.
        Achieved a MAE of 0.02, showing consistency in prediction accuracy across multiple stocks.

## Results Summary

    LSTM (Single Stock): MAE = 0.02
    Prophet: MAE = 16.2
    LSTM (Multi-Stock): MAE = 0.02

The LSTM model outperformed Prophet, with a significantly lower MAE for both single and multi-stock predictions.
How to Set Up and Run the Project
Requirements

## To run this project,  install these dependencies by running:

pip install numpy pandas matplotlib tensorflow fbprophet scikit-learn

## Running the Project

    Clone the repository or download the project files.
    Open untitled_7.ipynb in Jupyter Notebook or any compatible environment.
    Ensure the stock prices.csv file is in the same directory as the notebook.
    Run all cells to:
        Analyze the dataset.
        Preprocess the data (remove nulls and outliers).
        Train the LSTM model for both single and multi-stock predictions.
        Compare results with Prophet.

## Conclusion

This project demonstrates that LSTM is more effective than Prophet for stock price prediction in this particular dataset, with an MAE of 0.02 compared to Prophet's 16.2.
