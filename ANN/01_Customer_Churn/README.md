# 📊 Customer Churn Prediction using ANN

## 🚀 Project Overview
This project focuses on predicting **customer churn** using an **Artificial Neural Network (ANN)**. Customer churn prediction is a **binary classification problem**, where the goal is to identify whether a customer will leave a service or stay.

Accurately predicting churn helps businesses take proactive actions to **improve customer retention and reduce revenue loss**.

---

## 🎯 Objective
- Predict whether a customer will churn or not  
- Build a deep learning model using ANN  
- Understand customer behavior through data  
- Improve decision-making for retention strategies  

---

## 📂 Project Structure
```
01_Customer_Churn/
│
├── data/                # Dataset files
├── notebooks/           # Jupyter notebooks for EDA & training
├── model/               # Saved trained model
├── app.py               # Streamlit application
├── requirements.txt     # Dependencies
└── README.md            # Project documentation
```

---

## 🧠 Model Architecture (ANN)
- Input Layer  
- Hidden Layers (Dense + Activation)  
- Output Layer (Sigmoid for binary classification)  

ANN models are effective for capturing **complex patterns in customer behavior**.

---

## 🛠️ Tech Stack
- Python  
- TensorFlow / Keras  
- NumPy & Pandas  
- Scikit-learn  
- Matplotlib / Seaborn  
- Streamlit (for deployment)  

---

## 📊 Dataset Features
Typical features used in churn prediction:
- Credit Score  
- Geography  
- Gender  
- Age  
- Tenure  
- Balance  
- Number of Products  
- Active Status  
- Estimated Salary  

**Target Variable:**
- `Exited` (1 = Churn, 0 = Stay)

---

## 🔍 Workflow
1. **Data Preprocessing**
   - Handling missing values  
   - Encoding categorical variables  
   - Feature scaling  

2. **Exploratory Data Analysis (EDA)**
   - Understanding distributions  
   - Identifying important features  

3. **Model Building**
   - ANN model creation  
   - Training and validation  

4. **Model Evaluation**
   - Accuracy  
   - Confusion Matrix  
   - Precision / Recall  

5. **Deployment**
   - Streamlit app for real-time prediction  

---

## 📈 Results
- Achieved strong performance using ANN  
- Model successfully identifies high-risk customers  
- Useful for real-world business applications  

---

## 💻 How to Run the Project

### 1. Clone the repository
```bash
git clone https://github.com/Muhammad-Farhan1/DL-Projects.git
cd DL-Projects/ANN/01_Customer_Churn
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the application
```bash
streamlit run app.py
```

---

## 📌 Future Improvements
- Hyperparameter tuning  
- Use advanced models (XGBoost, LSTM)  
- Model explainability (SHAP)  
- Deployment on cloud (AWS / Heroku)  

---

## 🤝 Contributing
Feel free to fork this repository and contribute by improving the model or adding new features.

---

## 📬 Contact
**Muhammad Farhan**  
🔗 GitHub: https://github.com/Muhammad-Farhan1  
