# 📈 Amazon Stock Price Prediction using LSTM

This project leverages a Long Short-Term Memory (LSTM) deep learning model to predict Amazon stock prices based on a comprehensive set of technical indicators. The performance of the LSTM model is compared with a traditional Linear Regression model to highlight the advantages of using deep learning in time-series forecasting.

---

## 🧠 Objective

The goal of this project is to build a robust stock price prediction model using both traditional and deep learning techniques, and evaluate their effectiveness using standard regression metrics. It focuses on **Amazon (AMZN)** stock data fetched using the `yfinance` library.

---

## 📊 Features Used (13 Total)

The model was trained on a set of 13 carefully engineered features:

- **Price Indicators:** `Open`, `High`, `Low`, `Close`, `Volume`
- **Moving Averages:** `SMA_30`, `SMA_100`
- **Technical Indicators:** `RSI`, `MACD`, `ATR`
- **Volatility Measures:** `Volatility_30`
- **Bollinger Bands:** `Bollinger_High`, `Bollinger_Low`

All features were normalized before training for optimal model performance.

---

## 🤖 Models Compared

| Model             | Description                                      |
|------------------|--------------------------------------------------|
| Linear Regression| Baseline model to set performance benchmark      |
| LSTM             | Deep learning model to capture temporal patterns |

---

## 🧪 Evaluation Metrics

| Model            | RMSE | MAE   | R² Score |
|------------------|------|-------|----------|
| LSTM             | 4.28 | 3.213 | 0.9855   |   
| Linear Regression| 5.69 | 4.45  | 0.9707   |

The LSTM model significantly outperformed the Linear Regression model in all evaluation metrics.

# 📍 Predicted vs Actual Close Price (Next Day)

After training the model on 150 days of data, we tested it on completely **unseen 151st day** to simulate a real-world next-day prediction.


### 🔢 Result:
📍 Predicted Close Price: 195.16
📍 Actual Close Price: 194.95
> This highlights how the model performs on completely unseen real-world data.
> 🧠 Model was off by only **₹0.21**, showing high generalization capability even beyond the test set.


---

## 📈 Visualizations

- Actual vs Predicted closing prices
 ![image](https://github.com/user-attachments/assets/b616e5c0-52f6-4eb4-a3ab-7ed5c9dca4fb)
- 30-Day Forecast vs Actual
      Model's prediction for the next 30 days using latest available data.
  ![image](https://github.com/user-attachments/assets/0a3f2848-d9b8-449b-b39c-79a3b2922e12)
- Training and Validation Loss curve
  ![image](https://github.com/user-attachments/assets/db73e9ee-5470-4d04-a19e-0885efd1256d)

- Technical indicator plots (e.g., RSI, MACD, Bollinger Bands)
- ![image](https://github.com/user-attachments/assets/54b50d3f-1aee-4607-921d-42513743c89e)
- ![image](https://github.com/user-attachments/assets/df1ab550-51c9-473e-ae6e-d004d0c28f61)
- ![image](https://github.com/user-attachments/assets/e0635d35-7cb2-4529-97fa-d999bda0ee1e)
  


---

## 🔧 Tech Stack / Libraries

- `TensorFlow`, `Keras` – Model building
- `Pandas`, `NumPy` – Data preprocessing
- `Matplotlib`, `Seaborn` – Visualization
- `Scikit-learn` – Evaluation metrics
- `yfinance` – Data extraction

---

## 🚀 Future Scope

- ✅ Deploy as an interactive **Streamlit web app**
- 📊 Add more model comparisons (e.g., ARIMA, GRU)
- 🧠 Hyperparameter tuning using Keras Tuner
- 💾 Integrate live data updates using yfinance API

---

---

## 🙋‍♂️ Author

**Rishabh Yadav**

> “Code. Learn. Repeat.” 

> ⭐ If you liked this project, feel free to star the repo!



