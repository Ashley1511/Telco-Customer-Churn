# Telco-Customer-Churn
A machine learning project to predict customer churn using classification models and data visualization.

---

## 🗂 Project Overview

* **Objective**: Predict customer churn using demographic, service, and billing information.
* **Dataset**: [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
* **Tech Stack**: Python, pandas, scikit-learn, seaborn, matplotlib, Jupyter Notebook

---

## 📁 Folder Structure

```
Telco_Customer_Churn/
├── churn_analysis.ipynb         # Main notebook (EDA + modeling)
├── README.md                    # Project summary
├── requirements.txt             # Python dependencies
├── Telco_Customer_Churn_Dataset.csv  # Dataset 
└── screenshots/                 # Visualizations from the analysis
    ├── churn_distribution.png
    ├── correlation_heatmap.png
    └── gbm_feature_importance.png
```

---

## 🔍 Exploratory Data Analysis

Key insights uncovered:

* **26%** of customers have churned.
* Customers on **month-to-month contracts** and using **electronic check** are more likely to churn.
* **Higher monthly charges** and **shorter tenure** are strong churn indicators.

![Churn Distribution](screenshots/churn_distribution.png)

![Correlation Heatmap](screenshots/correlation_heatmap.png)

---

## 🧼 Preprocessing Steps

* Cleaned `TotalCharges` and converted to numeric
* One-hot encoded categorical features
* Scaled features using `StandardScaler`
* Handled missing values appropriately

---

## 🤖 Models Trained

| Model                 | Accuracy | Recall (Churn) | F1-Score (Churn) |
| --------------------- | -------- | -------------- | ---------------- |
| Logistic Regression   | 79%      | 52%            | 56%              |
| Random Forest         | 79%      | 50%            | 56%              |
| **Gradient Boosting** | **80%**  | **53%**        | **58%**          |

📌 Final model: **Gradient Boosting Classifier**

![Feature Importance](screenshots/gbm_feature_importance.png)

---

## 🧠 Business Insights

* Customers with **high bills**, **short tenure**, and **month-to-month contracts** are high-risk.
* Target retention campaigns at users with these patterns.
* Consider bundling or loyalty programs for new customers.

---

## 🧰 Tools Used

* `pandas`, `numpy` – data manipulation
* `matplotlib`, `seaborn` – data visualization
* `scikit-learn` – model training, evaluation
* `Jupyter Notebook` – interactive analysis

---

## 📦 How to Run

1. Clone the repo:

```bash
git clone https://github.com/Ashley1511/Telco_Customer_Churn.git
cd Telco_Customer_Churn
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook churn_analysis.ipynb
```

---

## 🙋‍♂️ Author

**Ashley Justin Denies**
[GitHub Profile](https://github.com/Ashley1511)

If you found this helpful, feel free to star ⭐ the repo or connect on LinkedIn!

---

## 🧩 License

This project is open-source and free to use for educational or portfolio purposes.
