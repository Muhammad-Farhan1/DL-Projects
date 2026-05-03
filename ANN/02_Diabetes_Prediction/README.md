# 🩺 Diabetes Prediction using Artificial Neural Network (ANN)

A deep learning project that predicts whether a patient has diabetes or not, using an Artificial Neural Network (ANN) built with TensorFlow/Keras. The model is trained on the **Pima Indians Diabetes Dataset** sourced from the National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK).

---

## 📌 Project Overview

This project is part of the **DL-Projects** repository under the `ANN` section. The goal is to classify patients as diabetic or non-diabetic based on several clinical health features. It covers the full machine learning pipeline:

- Exploratory Data Analysis (EDA)
- Data Preprocessing & Feature Scaling
- ANN Model Architecture Design
- Model Training & Evaluation
- Performance Metrics & Visualization

---

## 📂 Project Structure

```
02_Diabetes_Prediction/
│
├── diabetes_prediction.ipynb   # Main Jupyter Notebook
├── diabetes.csv                # Dataset (Pima Indians Diabetes Database)
├── model.h5                    # Saved trained model (if applicable)
└── README.md                   # Project documentation
```

---

## 📊 Dataset

- **Source:** [Kaggle – Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Original Source:** National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK)
- **Records:** 768 patients (all females, age ≥ 21, of Pima Indian heritage)
- **Target Variable:** `Outcome` — `1` (Diabetic) / `0` (Non-Diabetic)

### Features

| Feature                    | Description                                              |
|---------------------------|----------------------------------------------------------|
| `Pregnancies`             | Number of times the patient has been pregnant            |
| `Glucose`                 | Plasma glucose concentration (2-hour oral glucose test)  |
| `BloodPressure`           | Diastolic blood pressure (mm Hg)                         |
| `SkinThickness`           | Triceps skin fold thickness (mm)                         |
| `Insulin`                 | 2-hour serum insulin (mu U/ml)                           |
| `BMI`                     | Body Mass Index (weight in kg / height in m²)            |
| `DiabetesPedigreeFunction`| Likelihood of diabetes based on family history           |
| `Age`                     | Age of the patient (years)                               |
| `Outcome`                 | Target variable — 1: Diabetic, 0: Non-Diabetic           |

---

## 🧠 Model Architecture

The ANN is built using **TensorFlow/Keras** with the following layers:

```
Input Layer       →  8 features
Dense Layer 1     →  32 neurons, ReLU activation
Dense Layer 2     →  16 neurons, ReLU activation
Output Layer      →  1 neuron, Sigmoid activation (binary classification)
```

- **Loss Function:** Binary Crossentropy  
- **Optimizer:** Adam  
- **Metrics:** Accuracy  

---

## ⚙️ Technologies Used

| Tool / Library  | Purpose                          |
|----------------|----------------------------------|
| Python 3.x      | Programming Language             |
| TensorFlow / Keras | ANN Model Building & Training |
| NumPy           | Numerical computations           |
| Pandas          | Data loading & manipulation      |
| Matplotlib      | Plotting & visualization         |
| Seaborn         | Statistical data visualization   |
| Scikit-learn    | Preprocessing, train-test split, metrics |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Muhammad-Farhan1/DL-Projects.git
cd DL-Projects/ANN/02_Diabetes_Prediction
```

### 2. Install Dependencies

```bash
pip install tensorflow numpy pandas matplotlib seaborn scikit-learn
```

### 3. Run the Notebook

Open and run the Jupyter Notebook:

```bash
jupyter notebook diabetes_prediction.ipynb
```

---

## 📈 Results

The model is evaluated using the following metrics:

| Metric        | Value (Approx.) |
|---------------|-----------------|
| Training Accuracy | ~80–85%    |
| Validation Accuracy | ~76–80%  |
| Loss          | Binary Crossentropy |

> **Note:** Results may slightly vary due to random seed and initialization.

Evaluation includes:
- Accuracy and Loss curves (Training vs Validation)
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)

---

## 🔄 Workflow

```
Load Dataset
    ↓
Exploratory Data Analysis (EDA)
    ↓
Handle Missing / Zero Values
    ↓
Feature Scaling (StandardScaler)
    ↓
Train-Test Split (80/20)
    ↓
Build ANN Model
    ↓
Train Model
    ↓
Evaluate Model
    ↓
Visualize Results
```

---

## 📉 EDA Highlights

- Distribution plots for each feature
- Correlation heatmap to identify feature relationships
- Class imbalance analysis (`Outcome` distribution)
- Detection and handling of biologically impossible zero values (e.g., Glucose = 0)

---

## ⚠️ Disclaimer

This model is developed for **educational and research purposes only**. It should **not** be used as a substitute for professional medical diagnosis. Always consult a qualified healthcare provider for medical advice.

---

## 👤 Author

**Muhammad Farhan**  
GitHub: [@Muhammad-Farhan1](https://github.com/Muhammad-Farhan1)

---

## 📁 Part of DL-Projects

This project is part of the larger **DL-Projects** repository, which includes various deep learning implementations:

---

## 📄 License

This project is open-source and available under the [MIT License](../../LICENSE).
