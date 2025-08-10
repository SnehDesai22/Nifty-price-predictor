# Nifty Price Predictor

This project uses an LSTM (Long Short-Term Memory) neural network to predict the closing price of the Nifty index based on historical data.

## 📌 Project Overview
The goal of this project is to forecast the Nifty 50 index closing price using past historical data. The LSTM model is chosen because it can capture time-series dependencies better than traditional feedforward networks.

## 🚀 Features
- Data preprocessing with scaling (MinMaxScaler)
- LSTM-based model architecture
- Train/validation split
- Model evaluation using **MSE**, **RMSE**, and **R² Score**
- Actual vs Predicted price comparison
- CSV export of predictions

## 🛠 Technologies Used
- Python 3.x
- Pandas
- NumPy
- PyTorch
- Scikit-learn
- Matplotlib / Seaborn (for visualization)

## 📂 Project Structure
```
├── Nifty_price_predictor.ipynb   # Main Jupyter Notebook
├── predictions.csv               # Model predictions (optional output)
├── README.md                     # Project documentation
```
## 📊 How It Works
1. **Load Dataset** - Nifty 50 historical data is loaded from a CSV or API.
2. **Preprocess Data** - Missing values handled, features scaled using MinMaxScaler.
3. **Create Sequences** - Past `n` days used to predict the next day's closing price.
4. **Build LSTM Model** - Multi-layer LSTM with dropout for regularization.
5. **Train Model** - Optimize using Adam optimizer and MSE loss function.
6. **Evaluate Model** - Compare predicted vs actual prices.
7. **Save Predictions** - Export results to CSV.

## 📈 Example Output
| Date       | Actual_Close | Predicted_Close |
|------------|--------------|----------------|
| 2024-08-01 | 22450.15     | 22430.87       |
| 2024-08-02 | 22490.25     | 22460.93       |

## 🔮 Future Improvements
- Hyperparameter tuning for better accuracy
- Using additional features like volume, technical indicators
- Experimenting with GRU and Transformer models
- Deploy as a web app for real-time predictions

## 🧑‍💻 Author
Sneh Desai

