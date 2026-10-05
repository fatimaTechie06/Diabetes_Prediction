# 🩺 DiabetesAI – Diabetes Risk Prediction System

## 📌 Overview

**DiabetesAI** is a machine learning-based diabetes risk prediction system developed using **Python, Streamlit, and Scikit-learn**.

The application uses a **Decision Tree Classifier** to analyze eight clinical features and estimate the probability of diabetes. It provides an interactive dashboard for prediction, analytics, prediction history, dataset exploration, and model information.

> **Note:** This project is developed for educational, portfolio, and analytical demonstration purposes. It is not intended to provide medical diagnosis or treatment advice.

---

## 🎯 Objectives

* Predict diabetes risk using machine learning.
* Analyze important patient health parameters.
* Provide an interactive and user-friendly dashboard.
* Display diabetes probability and risk category.
* Maintain prediction history.
* Provide dataset exploration and analytics.
* Generate downloadable prediction reports.

---

## 🚀 Features

### 🔮 1. Diabetes Prediction

The system accepts the following **8 input features**:

1. Pregnancies
2. Glucose
3. Blood Pressure
4. Skin Thickness
5. Insulin
6. BMI
7. Diabetes Pedigree Function
8. Age

The model generates:

* Prediction result
* Diabetes probability
* Risk category
* Classification confidence
* Risk probability visualization
* Patient metric visualization

The application uses the trained model and feature list stored in `diabetes_model.pkl` and `diabetes_features.pkl`.

### 📊 2. Analytics Dashboard

The Analytics Hub provides:

* Total assessments
* Positive detections
* Negative detections
* Mean risk score
* Historical classification chart
* Risk-level distribution chart

### 📜 3. Prediction History

Each prediction can be stored with:

* Timestamp
* Patient input parameters
* Prediction
* Probability
* Risk level

The history is stored in:

```text
prediction_history.csv
```

### 🗂️ 4. Dataset Explorer

The Dataset Explorer provides:

* Total number of records
* Number of features
* Positive instances
* Dataset sample
* Feature distribution visualization

The application expects the training dataset as:

```text
diabetes.csv
```

### 🤖 5. Model Architecture

The project uses:

**Algorithm:** Decision Tree Classifier

**Configuration:**

| Parameter             | Value                    |
| --------------------- | ------------------------ |
| Algorithm             | Decision Tree Classifier |
| Max Depth             | 7                        |
| Minimum Samples Leaf  | 15                       |
| Minimum Samples Split | 2                        |
| Target Variable       | Outcome                  |
| Number of Features    | 8                        |

### 📥 6. Downloadable Reports

After a prediction, the application provides a downloadable CSV report containing the assessment result, probability, risk category, input parameters, and timestamp.

---

## 🧠 Machine Learning Workflow

```text
Dataset
   ↓
Data Preprocessing
   ↓
Feature Selection
   ↓
Model Training
   ↓
Decision Tree Classifier
   ↓
Model Evaluation
   ↓
Saved Model (.pkl)
   ↓
Streamlit Application
   ↓
User Input
   ↓
Diabetes Risk Prediction
   ↓
Probability & Risk Category
```

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Streamlit**
* **Plotly**
* **Pickle**
* **Jupyter Notebook**

The Streamlit application uses Pandas/NumPy for data processing and Plotly for interactive visualizations.

---

## 📁 Project Structure

```text
DiabetesAI/
│
├── app.py
├── diabetes_prediction.ipynb
├── diabetes.csv
├── diabetes_model.pkl
├── diabetes_features.pkl
├── prediction_history.csv
├── requirements.txt
└── README.md
```

### File Description

| File                        | Description                                          |
| --------------------------- | ---------------------------------------------------- |
| `app.py`                    | Main Streamlit application                           |
| `diabetes_prediction.ipynb` | Machine learning model development/training notebook |
| `diabetes.csv`              | Diabetes dataset                                     |
| `diabetes_model.pkl`        | Trained Decision Tree model                          |
| `diabetes_features.pkl`     | Stored feature ordering                              |
| `prediction_history.csv`    | Prediction history                                   |
| `requirements.txt`          | Required Python libraries                            |
| `README.md`                 | Project documentation                                |

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/DiabetesAI.git
```

### 2. Open the Project

```bash
cd DiabetesAI
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 📦 Requirements

Create a `requirements.txt` file containing:

```text
streamlit
pandas
numpy
scikit-learn
plotly
```

---

## 📊 Risk Classification

The application categorizes diabetes probability into four risk levels:

| Probability | Risk Level        |
| ----------: | ----------------- |
|       0–30% | 🟢 Low Risk       |
|      30–60% | 🟡 Moderate Risk  |
|      60–80% | 🟠 High Risk      |
|     80–100% | 🔴 Very High Risk |

These thresholds are implemented directly in the application.

---

## 🖥️ Application Modules

```text
🏠 Overview
    ↓
🔮 Prediction Engine
    ↓
📊 Analytics Hub
    ↓
📜 Prediction History
    ↓
🗂 Dataset Explorer
    ↓
🤖 Model Architecture
    ↓
📚 Clinical Insights
    ↓
ℹ️ About
```

The Streamlit sidebar provides these navigation modules.

---

## 🔬 Model Input Features

The model processes the following feature order:

```text
Pregnancies
Glucose
BloodPressure
SkinThickness
Insulin
BMI
DiabetesPedigreeFunction
Age
```

The application explicitly constructs the prediction input using this feature ordering.

---

## 📈 Visualization

The system uses interactive Plotly visualizations including:

* Risk Probability Gauge
* Patient Metric Radar Chart
* Historical Classification Pie Chart
* Risk-Level Distribution Chart
* Feature Distribution Histogram

---

## 🔐 Medical Disclaimer

This application is intended **only for educational, portfolio, and analytical demonstration purposes**.

It does not provide medical diagnosis, treatment recommendations, or clinical advice. Users should consult a qualified healthcare professional regarding personal medical conditions.

---

## ⭐ Future Enhancements

* Integration with a larger clinical dataset
* Additional machine learning algorithms
* Model performance comparison
* Feature importance visualization
* User authentication
* Cloud deployment
* Database integration
* PDF medical-style report generation
* Mobile-friendly interface

---

## 📄 License

This project is intended for educational and academic purposes.
