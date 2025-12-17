🐶 Dogecoin Price Prediction with Machine Learning

This project explores how different machine learning and time series models can be used to predict the closing price of Dogecoin using historical market data.

The goal is to analyze past price behavior, engineer meaningful features, train multiple models, and compare their performance to understand which approaches work best for cryptocurrency price forecasting.

📌 Project Overview

Cryptocurrency prices are highly volatile and difficult to predict. In this project, we use historical Dogecoin price data and apply several machine learning and deep learning models to forecast future prices.

The project includes:

Data preprocessing and feature engineering

Multiple prediction models

Performance comparison using standard metrics

Visualization of predictions vs actual prices

📊 Dataset

The dataset contains historical Dogecoin price data with the following columns:

Date

Open

High

Low

Close

Adjusted Close

Volume

Time period: Nov 2017 – Sep 2022

Total records after cleaning: 1,760 rows

Missing values were removed to ensure data consistency.

🛠 Feature Engineering

To improve prediction accuracy, several features were created:

Lag_1 – Previous day’s closing price

MA7 – 7-day moving average

MA21 – 21-day moving average

Daily Returns

7-day Rolling Volatility

After correlation analysis, the most effective features selected were:

Lag_1

MA7

MA21

🤖 Models Used

The following models were trained and evaluated:

Machine Learning Models

Linear Regression

Random Forest Regressor

XGBoost Regressor

Time Series Models

ARIMA

LSTM (Long Short-Term Memory Neural Network)

Each model was trained using an 80/20 train-test split.

📈 Performance Metrics

Models were evaluated using:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

R² Score

🏆 Results Summary
Model	R² Score	Observation
Linear Regression	0.9863	Best overall performance
LSTM	0.9787	Best deep learning model
XGBoost	0.9651	Strong non-linear model
Random Forest	0.8874	Struggled with volatility
ARIMA	-0.0027	Not suitable for crypto data
Key Findings:

Linear Regression surprisingly performed the best

LSTM captured long-term dependencies well

ARIMA failed due to high volatility

Feature engineering played a crucial role in accuracy

📉 Visualizations

The project includes:

Closing price trends

Moving averages

Daily returns

Volatility plots

Actual vs predicted price graphs for each model

🧪 Tools & Technologies

Language: Python

Libraries:

Pandas, NumPy

Scikit-learn

XGBoost

TensorFlow / Keras

Statsmodels

Environment: Jupyter Notebook

🚀 How to Run

Clone the repository

git clone https://github.com/yourusername/dogecoin-price-prediction.git


Install dependencies

pip install -r requirements.txt


Open the Jupyter Notebook and run cells sequentially

jupyter notebook


Upload the Dogecoin historical CSV file when prompted

⚠️ Limitations

Uses historical price data only

No real-time predictions

External factors like social media sentiment are not included

Predictions are not financial advice

🔮 Future Improvements

Add real-time price prediction

Include social media sentiment analysis

Explore transformer-based models

Deploy as a web app or API

Improve long-term forecasting stability

📜 License

This project is for educational and research purposes.

🙌 Author

Dilawer Khan
