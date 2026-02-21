# Rene_Wind
# 🌬️ ReneWind – Wind Turbine Failure Prediction Using Machine Learning

## 📖 Project Overview

Renewable energy sources are becoming a critical part of the global energy ecosystem as organizations work toward reducing environmental impact. Among renewable sources, **wind energy** is one of the most mature and widely adopted technologies.

Wind turbines operate under harsh environmental conditions, and unexpected generator failures can lead to **high maintenance and replacement costs**. To reduce these costs, companies are increasingly adopting **predictive maintenance** strategies powered by machine learning.

In this project, I worked as a **Data Scientist at ReneWind**, a company focused on improving wind energy production through data-driven solutions. Using historical sensor data collected from wind turbines, I built classification models to **predict generator failures before they occur**.

---

## 🎯 Business Objective

The main objectives of this project are:

- Predict wind turbine generator failures in advance
- Reduce costly generator replacements by early detection
- Optimize maintenance scheduling using predictive insights
- Minimize operational and maintenance costs

---

## ⚙️ Predictive Maintenance Context

Predictive maintenance uses **sensor data and analytical models** to detect early signs of component degradation.  
In this project, the prediction outcomes translate into real-world costs:

- **True Positive (TP):** Failure correctly predicted → Repair cost  
- **False Negative (FN):** Failure missed → Replacement cost (very high)  
- **False Positive (FP):** Failure predicted but none exists → Inspection cost  

Since replacement costs are much higher than repair or inspection costs, the model is designed to **minimize false negatives**.

---

## 🗂 Dataset Description

- Sensor-based, ciphered dataset to protect proprietary information
- 40 predictor variables collected from turbine sensors
- Binary target variable:
  - `1` → Generator failure
  - `0` → No failure

### Dataset Files
- **Train.csv:** 20,000 observations (used for training and tuning)
- **Test.csv:** 5,000 observations (used only for final evaluation)

---

## 🛠 Tools & Technologies Used

- **Programming Language:** Python  
- **Environment:** Google Colab / Jupyter Notebook  
- **Libraries Used:**
  - pandas – data handling
  - numpy – numerical operations
  - matplotlib & seaborn – visualization
  - scikit-learn – ML models and evaluation

---

## 🔍 Project Workflow & Work Done

The project follows an end-to-end machine learning lifecycle.

---

### 1️⃣ Data Understanding & Preparation

- Loaded and inspected training and test datasets
- Verified dataset dimensions and data types
- Checked class imbalance in the target variable
- Ensured data consistency and readiness for modeling

---

### 2️⃣ Exploratory Data Analysis (EDA)

EDA was performed to understand patterns and variability in sensor readings.

Key steps included:
- Distribution analysis of sensor features
- Identification of correlations between predictors
- Comparison of sensor behavior for failure vs non-failure cases

Visualizations were used to gain better intuition about the data.

---

### 3️⃣ Data Preprocessing

- Feature scaling where required
- Handling class imbalance using suitable techniques
- Separation of predictors and target variable
- Splitting data into training and validation sets

---

### 4️⃣ Model Building

Several classification models were trained and compared, including:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- (Optional) Gradient Boosting models

Hyperparameter tuning was performed to improve model performance.

---

### 5️⃣ Model Evaluation

Models were evaluated using:
- Confusion matrix
- Precision, Recall, and F1-score
- Focus on **Recall for failure class (1)** to reduce false negatives

The final model was selected based on **business cost considerations**, not just accuracy.

---

## 📊 Key Insights from the Analysis

- Certain sensor patterns strongly indicate early-stage generator failures
- Ensemble models outperform simpler models in failure detection
- Recall for failure detection is more critical than overall accuracy
- Early detection significantly reduces high replacement costs

---

## 💡 Business Recommendations

Based on the analysis and model performance:

- Use the trained model for real-time failure monitoring
- Schedule preventive maintenance for high-risk generators
- Prioritize reducing false negatives to avoid costly breakdowns
- Integrate model predictions into turbine monitoring systems

---

## 📁 Repository Structure
│
├── ReneWind.ipynb
├── ReneWind.html
└── README.md
└── Train.csv
└── Test.csv

---

## 📌 Conclusion

This project demonstrates how **machine learning can enable predictive maintenance** in the renewable energy sector. By accurately identifying potential generator failures, ReneWind can reduce downtime, avoid expensive replacements, and improve overall operational efficiency.

The project highlights the importance of aligning ML evaluation metrics with **real-world business costs**, making it a practical and impactful data science solution.

---

## 👤 Author

**Rahul Naidu**  
B.Tech – Computer Science (2022)  
Aspiring Data Scientist / Business Analyst  

---

⭐ If you found this project helpful, feel free to star the repository!
