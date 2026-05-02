# 🔋 Smart Battery Health Prediction & Recommendation System

## 📌 Overview

This project was developed as part of my Artificial Intelligence & Machine Learning (AIML) coursework under the Machine Learning using Python (MDM) subject during my Third Year B.Tech (Electronics Engineering) at Walchand College of Engineering, Sangli.

It demonstrates practical application of machine learning concepts including data preprocessing, feature engineering, regression modeling, and performance evaluation on a real-world problem.

It analyzes device usage patterns, charging behavior, and environmental factors to estimate battery degradation and suggest next steps:

* ✅ Keep Using
* 🔧 Replace Battery
* 📱 Change Phone

---

## 🎯 Problem Statement

Smartphone batteries degrade over time due to:

* Charging cycles
* Temperature variations
* Heavy usage patterns

Accurately predicting battery health helps improve:

* Device reliability
* User decision-making
* Preventive maintenance

---

## 📊 Dataset

* Source: Kaggle (Smartphone Battery Dataset)
* Size: ~5000 records
* Features: 17 input features

### Input Features:

* Device age
* Charging cycles
* Battery temperature
* Screen usage
* Fast/overnight charging
* Background app usage
* Signal strength

### Target:

* Battery Health (%) → Regression
* Recommended Action → Classification

---

## ⚙️ Machine Learning Pipeline

### 1. Data Preprocessing

* Removed missing values and duplicates
* Encoded categorical variables
* Performed statistical analysis & visualization

### 2. Feature Engineering

* Selected numerical features
* Removed multicollinearity using **VIF**
* Outlier detection using **Cook’s Distance**

### 3. Model Development

* Linear Regression (Baseline Model)
* KNN Regressor (k=5)

### 4. Model Evaluation

* Metrics used:

  * R² Score
  * MAE
  * RMSE
* Cross-validation applied
* Overfitting check performed

---

## 📈 Results

| Model             | Performance                              |
| ----------------- | ---------------------------------------- |
| Linear Regression | High accuracy, best performance          |
| KNN (k=5)         | Good performance, captures non-linearity |

👉 **Final Model Selected: Linear Regression**

---

## 🔍 Key Insights

* Battery health decreases with **device age**
* Frequent charging → faster degradation
* High temperature negatively impacts battery life
* Heavy usage (gaming/streaming) reduces health

---

## 🧠 Recommendation System

Based on predicted battery health:

| Battery Health | Recommendation  |
| -------------- | --------------- |
| > 75%          | Keep Using      |
| 45% – 75%      | Replace Battery |
| < 45%          | Change Phone    |

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Statsmodels
* Matplotlib, Seaborn

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/your-username/repo-name.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the script

```bash
python battery_health_prediction.py
```

---

## ⚠️ Challenges & Limitations

* Data leakage initially identified and fixed
* Some features were highly correlated (handled using VIF)
* Model depends on dataset quality
* Real-world conditions may vary

---

## 🔐 Ethical Considerations

* Ensures user data privacy
* Predictions are advisory, not absolute decisions
* Avoids biased or misleading outputs

---

## 👨‍💻 Author

**Shreyas Kamble**
Electronics Engineering Student | Embedded Systems +  VLSI Enthusiast

---

## ⭐ Future Improvements

* Deploy as a web dashboard (Streamlit)
* Integrate real-time mobile data
* Add deep learning models
* Improve dataset diversity

---
