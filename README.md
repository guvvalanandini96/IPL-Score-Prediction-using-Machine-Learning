# IPL-Score-Prediction-using-Machine-Learning


This project focuses on predicting the final score of an IPL (Indian Premier League) match innings using Machine Learning techniques. The model is trained on historical IPL data and predicts the total score based on match conditions.

---

## 🎯 Objective

To build a machine learning model that predicts the final score of a batting team using features like runs, wickets, overs, and team information.

---

## 📂 Dataset Description

The dataset contains ball-by-ball IPL match data including:

* Batting Team
* Bowling Team
* Overs
* Runs scored
* Wickets fallen
* Runs in last 5 overs
* Wickets in last 5 overs
* Match date
* Final total score

---

## ⚙️ Project Workflow

### 🔹 Data Preprocessing

* Removed irrelevant columns (match_id, venue, players, etc.)
* Filtered consistent IPL teams
* Removed initial overs (first 5 overs)
* Converted date column into datetime format

---

### 🔹 Feature Engineering

* Selected important features using correlation analysis
* Applied **One-Hot Encoding** for categorical variables (teams)

---

### 🔹 Train-Test Split

* Training Data → IPL seasons (2008–2016)
* Testing Data → IPL season (2017)

---

## 🤖 Models Used

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* AdaBoost Regressor

---

## 📊 Model Evaluation

Evaluation Metrics:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)

👉 **Linear Regression performed best with lowest error**

---

## 🔍 Predictions

The model predicts final scores based on:

* Batting team
* Bowling team
* Overs
* Runs
* Wickets
* Last 5 overs performance

### Example Predictions:

* KKR vs DD → 200/9
* SRH vs RCB → 146/10
* MI vs KXIP → 186/8
* RR vs CSK → 151/7

---

## 🛠 Tools & Libraries

* Python
* pandas
* numpy
* scikit-learn
* matplotlib
* seaborn

---

## 📁 Project Files

* project.ipynb → Jupyter Notebook
* ipl.csv → Dataset
* requirements.txt → Libraries used

---

## 🚀 How to Run

1. Install dependencies:

```id="mlcmd1"
pip install -r requirements.txt
```

2. Run notebook:

```id="mlcmd2"
jupyter notebook
```

---

## 📊 Key Insights

* Recent performance (last 5 overs) strongly affects final score
* Team combinations influence scoring patterns
* Linear models can perform well with structured cricket data

---

## 🎯 Conclusion

This project demonstrates how machine learning can be applied to sports analytics. It successfully predicts IPL scores using historical data and regression models.

---

## 🔮 Future Improvements

* Use advanced models (XGBoost, Neural Networks)
* Add more recent IPL data
* Perform hyperparameter tuning

---

⭐ This project is part of my Machine Learning portfolio.
