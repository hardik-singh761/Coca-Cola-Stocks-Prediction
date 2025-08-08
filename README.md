📈 Coca-Cola Stock Prediction – Live & Historical
📌 Project Overview
This project predicts Coca-Cola's (KO) stock prices using historical market data and live stock feeds. The goal is to blend machine learning with time-series forecasting for real-world financial predictions.

The pipeline supports both offline training and live streaming predictions, making it suitable for dashboards, automated alerts, and investment analysis.

🛠 Tools & Technologies
Programming Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, YFinance

Algorithms: Random Forest Regressor

Data Sources: Yahoo Finance API (yfinance)

Other Tools: SQL, Excel for data storage and analysis

📂 Dataset
Source: Yahoo Finance – Ticker Symbol: KO

Date Range: Jan 2015 – Dec 2024

Columns: Date, Open, High, Low, Close, Volume

Additional engineered features:

MA_20 & MA_50: 20-day & 50-day moving averages

Daily_Return: Percentage change in closing price

Volatility: 20-day rolling standard deviation of daily returns

📊 Features Implemented
Data Collection:

Downloaded historical Coca-Cola stock data via yfinance

Pulled real-time market data for live predictions

Exploratory Data Analysis (EDA):

Correlation heatmaps

Price trends & moving averages

Volatility visualization

Feature Engineering:

Rolling averages (MA_20, MA_50)

Daily returns

Rolling volatility

Model Building:

Random Forest Regressor

MinMax scaling for features

Train/Test split without shuffling for time-series integrity

Evaluation Metrics:

Mean Squared Error (MSE)

Mean Absolute Error (MAE)

Live Predictions:

Fetches the latest stock data

Applies the trained model to predict today’s closing price

📈 Example Prediction Output
text
Copy
Edit
Predicted Closing Price: 61.74 USD
📌 How to Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/coca-cola-stock-prediction.git
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the training script:

bash
Copy
Edit
python train_model.py
Run the live prediction script:

bash
Copy
Edit
python live_predict.py
📅 Future Improvements
Integrate ARIMA/LSTM for time-series forecasting

Add hyperparameter tuning with GridSearchCV

Create an interactive dashboard with Streamlit or Power BI

Include multi-stock prediction capability

📜 License
This project is licensed under the MIT License – feel free to use and modify.
