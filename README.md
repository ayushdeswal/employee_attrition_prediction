# 📊 Predictive People Analytics: HR Employee Attrition Model

**Author:** [Ayush Deswal]  
**Tools Used:** Python, Pandas, Scikit-Learn, Seaborn, Matplotlib  

---

## 📑 Project Overview
Employee turnover is a massive expense for organizations, with replacement costs reaching up to 200% of an employee's annual salary due to recruitment, onboarding, and lost productivity. 

This project transitions Human Resources from reactive, "gut-feeling" management to proactive **Predictive People Analytics**. By analyzing historical workforce data, this project successfully answers two critical business questions:
1. **Why are employees leaving?** (Identifying the root causes of attrition).
2. **Who is likely to leave next?** (Building a predictive machine learning model to flag high-risk employees).

## 🎯 Key Objectives & Workflow
1. **Data Preprocessing:** Cleaned and formatted HR data, applying Label Encoding for ordinal variables and One-Hot Encoding for nominal variables. Scaled numerical features for optimal machine learning performance.
2. **Exploratory Data Analysis (EDA):** Conducted visual investigations to uncover the underlying patterns driving turnover, focusing on commute distances, compensation, overtime burden, and departmental differences.
3. **Predictive Modeling:** Trained and evaluated **Logistic Regression** and **Random Forest** classification algorithms. Addressed an 84/16 class imbalance using `class_weight='balanced'` and prioritized **Recall** to ensure true flight-risk employees were not missed.
4. **Strategic Insight Generation:** Extracted Feature Importance to rank the top drivers of attrition and generated a live "Watch List" of active employees with a >70% probability of resigning.

## 📂 Repository Structure & Deliverables

This repository contains the three core deliverables required for this project:

* `HR_Attrition_Analysis.ipynb`: The primary Jupyter Notebook containing the end-to-end Python code, narrative markdown, EDA visualizations, and model training.
* `employee_attrition_model.pkl` & `employee_data_scaler.pkl`: The exported Logistic Regression model object and data scaler. These allow HR software engineers to deploy the model and score new employee data without re-running the analysis.
* `Executive_HR_Report.pdf`: A non-technical, corporate-facing memo summarizing the top attrition drivers, departmental risk breakdowns, and data-backed retention strategies.

## 💡 Key Business Insights
Through rigorous Exploratory Data Analysis and Random Forest feature importance extraction, the top drivers of employee attrition were identified:

1. **Compensation & Age:** Employees under 30 and those with lower Monthly Incomes relative to their peers represent the highest flight risk.
2. **The Overtime Burden:** Employees logging frequent "OverTime" are nearly **3x more likely to quit** compared to those working standard hours.
3. **Departmental Friction:** Sales Representatives exhibit an alarming turnover rate of ~40%. The R&D department features the highest aggregate volume of flight risks.
4. **Commute Distance:** The probability of attrition spikes significantly for employees commuting more than 15 miles.

**Recommendations:** Implement an HR "Overtime Cap," restructure entry-level compensation for Sales Reps and Lab Techs, and offer a 2-day remote work option for employees with long commutes.

## ⚙️ How to Run This Project

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git)
   ```
2. Ensure you have the required Python libraries installed:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. Open `HR_Attrition_Analysis.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
4. Run all cells to process the data, view the EDA charts, train the models, and generate the final HR Watch List.

**Note:** The dataset used for this analysis is the standard IBM HR Analytics Employee Attrition & Performance dataset, which contains 1,470 employee records and 35 features.
