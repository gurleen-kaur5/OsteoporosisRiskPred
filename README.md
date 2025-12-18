# 🦴 OsteoPred – Predictive Modeling of Osteoporosis Risk

## 📌 Project Overview

**OsteoPred** is an end-to-end **Machine Learning + Web Application** project that predicts the **risk of osteoporosis** using clinical features. The project benchmarks multiple classifiers and identifies **CatBoost** as the best-performing model. The final solution is deployed as a **Flask-based web application** with model explainability using **SHAP**.

This repository is also used as a **DevOps / SCM (Git) demonstration project**, showcasing advanced Git concepts such as **branching, merging, rebasing, stashing, tagging, and comparison commands**.

---

## 🎯 Objectives

* Build a reliable ML model for osteoporosis risk prediction
* Compare multiple classifiers and select the best model
* Ensure **high precision** to minimize false positives
* Provide **model explainability** using SHAP
* Deploy the model via a **Flask web application**
* Demonstrate **professional Git workflows** for SCM

---

## 🧠 Machine Learning Pipeline

### 🔹 Dataset

* Balanced clinical dataset
* **1,954 records**, **14 features**
* Preprocessed and cleaned before training

### 🔹 Models Evaluated

* Logistic Regression
* Random Forest
* XGBoost
* LightGBM
* AdaBoost
* Gradient Boosting
* Extra Trees
* Support Vector Machine
* **CatBoost (Best Model)**

### 🔹 Final Model (CatBoost)

* **Mean CV AUC-ROC:** 0.9231
* **F1 Score:** 0.8703
* **Precision:** 1.0000 (Zero False Positives)

---

## 🔍 Model Explainability (XAI)

The project integrates **SHAP (SHapley Additive exPlanations)** to ensure transparency and trust:

* Global feature importance plot
* SHAP beeswarm plot for individual feature contributions

---

## 🌐 Web Application Architecture

### 🔹 Backend

* **Flask** REST API
* Loads trained CatBoost model (`.cbm`)
* Accepts user input and returns predictions

### 🔹 Frontend

* HTML, CSS, JavaScript
* User-friendly form for clinical inputs
* Real-time prediction results

---

## 📁 Project Structure

```
├── osteopred.ipynb                  # EDA and experimentation
├── modeltrain.py                   # Model training & evaluation
├── final_catboost_model.cbm        # Trained CatBoost model
├── catboost_info/                  # CatBoost training logs
├── app.py                          # Flask backend
├── index.html                      # Frontend UI
├── style.css                       # Styling
├── script.js                       # Frontend logic
└── README.md                       # Project documentation
```

---

## ⚙️ Git & DevOps Workflow (Key Highlight)

This project demonstrates **advanced Git concepts**:

### 🔹 Source Code Management

* Git used for version control and collaboration
* Clean commit history and structured repository

### 🔹 Branching Strategy

* `main` → stable production-ready code
* `feature/ml-pipeline` → ML development
* `feature/backend-api` → Flask backend
* `feature/frontend-ui` → UI development

### 🔹 Merging

* Non-fast-forward merges to preserve feature history

### 🔹 Rebasing

* Used before merging feature branches to maintain a clean, linear history

### 🔹 Stashing

* Temporary storage of incomplete work during branch switching

### 🔹 Tagging

* Annotated tags used for versioning and releases

```bash
git tag -a v1.0 -m "Stable ML + Flask Deployment"
```

---

## 🚀 How to Run the Project Locally

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/gurleen-kaur5/OsteoporosisRiskPred
cd osteopred
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run Flask App

```bash
python app.py
```

### 4️⃣ Open in Browser

```
http://127.0.0.1:5000/
```

---

## 🧪 Results & Insights

* CatBoost outperformed all baseline models
* High precision ensures clinical safety
* SHAP enhances interpretability for healthcare use

---

## 🔮 Future Scope

* Integration with hospital EHR systems
* Real-time clinical decision support
* Model monitoring and retraining pipeline
* Docker & CI/CD deployment

---

## 🧑‍💻 Author

**Gurleen Kaur**
3rd Year CSE Undergraduate
Machine Learning | Data Science | Full Stack Development

---

## 📜 License

This project is for **academic and educational purposes**.
