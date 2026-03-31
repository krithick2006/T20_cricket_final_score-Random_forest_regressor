# 🏏  T20 Cricket Final Score Prediction

## 📌 Project Overview

This project predicts the **final score of a cricket innings** using machine learning.
The model takes simple match inputs like current runs, wickets lost, and ball number to estimate the final score.

---

## 🎯 Objective

To build a regression-based ML model that can:

* Predict final score in real-time
* Use minimal inputs
* Provide quick and accurate estimates

---

## 📊 Dataset

The dataset contains the following features:

| Feature     | Description                           |
| ----------- | ------------------------------------- |
| runs        | Current runs scored                   |
| wickets     | Wickets lost                          |
| ball        | Current ball (1–120 for T20 format)   |
| final_score | Final innings score (target variable) |

* Dataset is synthetically generated based on realistic cricket scoring patterns
* Suitable for training and testing ML models

---

## 🧠 Machine Learning Model

We use:

### ✅ Random Forest Regressor
### 🧠 Why Random Forest Regressor is Used

* **Captures Nonlinear Relationships**
  Cricket scoring depends on match situations like wickets and overs, which are not linear.
  Random Forest can model these complex patterns effectively.

* **Handles Match Dynamics Well**
  It understands scenarios like early wickets slowing scoring or death overs increasing runs.
  This makes predictions more realistic.

* **Reduces Overfitting**
  A single decision tree may memorize the data and perform poorly on new inputs.
  Random Forest averages multiple trees, reducing errors and improving generalization.

* **Provides Stable and Accurate Predictions**
  Since predictions are averaged across many trees, results are more consistent.
  This improves reliability compared to individual models.

* **Works Well with Few Features**
  Even with just runs, wickets, and ball, it can learn meaningful patterns.
  No need for complex feature engineering.

* **Minimal Data Preprocessing Required**
  It does not require scaling or normalization of data.
  This makes it easy and fast to implement.

* **Handles Noisy Data**
  Real-world cricket data can be inconsistent or noisy.
  Random Forest is robust and less affected by such variations.

* **Easy to Use with Good Performance**
  It requires less tuning compared to advanced models like XGBoost.
  Still delivers strong performance for this type of problem.

## ▶️ Example

Input:

```
Runs: 85  
Wickets: 3  
Ball: 70
```

Output:

```
Predicted Final Score: 178
```

---

## 📈 Future Improvements

* Use real-world datasets (IPL / Cricsheet)
* Add more features:

  * Run rate
  * Last 5 overs performance
  * Team & venue data
* Improve accuracy with:

  * XGBoost / LightGBM
* Deploy as:

  * Web app (Flask / Streamlit)
  * Mobile app

---

## 🧩 Project Structure

```
├── cricket_ml_dataset.csv
├── model.py
├── README.md
```

---

## 💡 Conclusion

This project demonstrates how machine learning can be applied to sports analytics using simple inputs.
Even with minimal features, the model can provide meaningful predictions for cricket matches.

---


KRITHICK
