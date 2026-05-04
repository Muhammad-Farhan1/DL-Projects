# 📈 Stock Price Prediction using RNN (LSTM)

A deep learning project that uses a **Recurrent Neural Network (RNN)** with **Long Short-Term Memory (LSTM)** cells to predict future stock prices based on historical time-series data.

---

## 🧠 Model Overview

This project implements an LSTM-based RNN to capture **temporal dependencies** in sequential stock price data. LSTMs are well-suited for time-series forecasting because they can retain information over long sequences, overcoming the vanishing gradient problem common in vanilla RNNs.

---

## 📁 Project Structure

```
01_Stock_Price_Prediction/
│
├── Stock_Price_Prediction.ipynb   # Main Jupyter Notebook
├── dataset/                       # Stock price CSV data
│   └── *.csv
└── README.md
```

---

## 📊 Dataset

- **Source:** [Yahoo Finance](https://finance.yahoo.com/) / Kaggle
- **Features used:** `Open`, `High`, `Low`, `Close`, `Volume`
- **Target variable:** `Close` price
- Historical stock data is split into **training** and **test** sets

---

## 🔧 Tech Stack

| Library        | Purpose                          |
|----------------|----------------------------------|
| Python 3.x     | Core language                    |
| NumPy          | Numerical computations           |
| Pandas         | Data manipulation                |
| Matplotlib     | Data visualization               |
| Scikit-learn   | Preprocessing (MinMaxScaler)     |
| TensorFlow / Keras | Building & training the LSTM model |

---

## 🏗️ Model Architecture

```
Input Layer       →  (timesteps, features)
LSTM Layer 1      →  units=50, return_sequences=True
Dropout           →  rate=0.2
LSTM Layer 2      →  units=50, return_sequences=False
Dropout           →  rate=0.2
Dense Layer       →  units=1 (predicted Close price)
```

- **Loss Function:** Mean Squared Error (MSE)  
- **Optimizer:** Adam  
- **Epochs:** 50  
- **Batch Size:** 32

---

## ⚙️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/Muhammad-Farhan1/DL-Projects.git
cd DL-Projects/RNN/01_Stock_Price_Prediction
```

### 2. Install Dependencies

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow
```

### 3. Open the Notebook

```bash
jupyter notebook Stock_Price_Prediction.ipynb
```

Run all cells from top to bottom.

---

## 📉 Results

The model predicts the stock's **closing price** and plots actual vs. predicted values for visual comparison.

- The LSTM captures the **overall trend** and **short-term patterns** effectively
- Performance is measured using **RMSE** (Root Mean Squared Error)

---

## 📌 Key Concepts

- **Time-series windowing:** Using past `n` days to predict the next day's price
- **Min-Max Normalization:** Scaling features to [0, 1] for stable training
- **Sequence modeling:** LSTM processes data step-by-step while maintaining memory

---

## ⚠️ Disclaimer

> Stock price prediction is inherently uncertain. This project is built for **educational purposes only** and should **not** be used as financial advice.

---

## 👤 Author

**Muhammad Farhan**  
📂 [GitHub Profile](https://github.com/Muhammad-Farhan1)

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
