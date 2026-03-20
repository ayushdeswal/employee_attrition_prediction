# 📊 Strategic People Analytics: Predicting Employee Attrition

![Python](https://img.shields.io/badge/python-3.8+-blue.svg) ![Scikit-Learn](https://img.shields.io/badge/sklearn-latest-orange.svg) ![Pandas](https://img.shields.io/badge/pandas-data_analysis-green.svg) ![License](https://img.shields.io/badge/license-MIT-blue.svg)

## 🎯 Business Context
Employee turnover is a critical challenge, with replacement costs reaching up to **200% of an annual salary** per lost employee. This project transitions HR management from "gut feeling" to **People Analytics**, providing a data-driven approach to workforce retention.

Using the IBM HR Analytics dataset, this project identifies the root causes of turnover and builds a predictive model to flag high-risk employees before they resign.

## 🚀 Key Features
* **Exploratory Data Analysis (EDA):** Deep-dive visualizations into the "Why" behind attrition (Overtime, Income, Tenure, and Commute).
* **Advanced Preprocessing:** Implementation of Label Encoding for ordinal data and One-Hot Encoding for nominal features.
* **Predictive Modeling:** Comparison between Logistic Regression (optimized for **Recall**) and Random Forest (optimized for **Feature Importance**).
* **Proactive Retention:** Automatically generates a **"High-Priority Watch List"** of active employees with a >70% probability of leaving.
* **Production Ready:** Exported model and scaler objects (`.pkl`) for immediate deployment into HR dashboards.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:**
  * **Pandas & NumPy:** Data manipulation and numerical analysis.
  * **Seaborn & Matplotlib:** Statistical data visualization.
  * **Scikit-Learn:** Machine learning, preprocessing, and evaluation.
  * **Joblib:** Model serialization for deployment.

## 📁 Project Structure

* `HR-Employee-Attrition.csv` - Dataset (IBM HR Analytics)
* `attrition_model.pkl` - Trained Logistic Regression model
* `data_scaler.pkl` - Scaler object for preprocessing new data
* `HR_Attrition_Analysis.ipynb` - Full end-to-end analysis & modeling
* `Strategic_Retention_Report.pdf` - Non-technical executive summary
* `requirements.txt` - List of dependencies

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/ayushdeswal/employee_attrition_prediction.git](https://github.com/ayushdeswal/employee_attrition_prediction.git)
   cd employee_attrition_prediction
   ```

2. **Create a virtual environment** (Optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## 📊 Key Insights & Results
* **The Overtime Trigger:** Employees working overtime are **nearly 3x more likely** to leave.
* **The Retention Danger Zone:** Attrition peaks between **Years 2 and 5** of tenure, suggesting a "Market Value Gap."
* **Departmental Crisis:** The **Sales Representative** role exhibits a turnover rate of **~40%**, requiring immediate structural intervention.
* **Model Performance:** The Logistic Regression model achieved a **Recall of XX%** *(Note: fill this in from your results)*, ensuring that the majority of flight-risks are captured by HR.

## 💡 Strategic Recommendations
* **Flexible Work Credits:** Offset the "Commute Tax" by offering remote work to employees living >15 miles away.
* **Tenure-Based Bonuses:** Implement retention milestones at the 18-month and 36-month marks for high-risk roles (Sales/R&D).
* **Overtime Audits:** Mandatory workload reviews for any employee logging >3 months of consistent overtime.
