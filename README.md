# 📊 End-to-End HR Employee Attrition Analytics

## 🎯 Project Overview
Employee turnover is a major cost for businesses. This project provides a comprehensive, end-to-end data analysis workflow to uncover the root causes of employee attrition using a real-world HR dataset of 1,470 employee records[cite: 1, 2]. 

Instead of relying on basic assumptions, this project combines **Rigorous Statistical Hypothesis Testing** with **Advanced Data Visualization** to deliver actionable business insights that HR managers can use to improve retention strategies[cite: 1, 2].

---

## 📂 Project Structure
The analysis is divided into two main phases, documented in separate Jupyter Notebooks:

### 🛠️ Part 1: Data Cleaning & Statistical Analysis (`HR_Data_Cleaning_and_Statistical_Analysis.ipynb`)
This notebook establishes the scientific foundation of the project by preparing the data and validating business questions statistically[cite: 2].
* **Data Quality Check:** Verified the integrity of the dataset, successfully achieving 0 missing values and 0 duplicates[cite: 2]. Non-value-adding columns were dropped to streamline the data[cite: 2].
* **Outlier Detection:** Implemented the IQR (Interquartile Range) method to identify anomalies in numerical variables such as Monthly Income and Years At Company[cite: 2].
* **Hypothesis Testing:** Utilized `SciPy` to run statistical tests[cite: 2]:
  * **Welch's T-Test:** Proved statistically significant differences in Age, Monthly Income, and Total Working Years between employees who left and those who stayed[cite: 2].
  * **Chi-Square Contingency Test:** Validated the strong relationship between Attrition and categorical factors like OverTime, Department, and Job Role[cite: 2].
* **Output:** Exported a fully prepared dataset (`Cleaned_HR_Data.csv`) for the visualization phase[cite: 2].

### 📈 Part 2: Data Visualization & Executive Dashboard (`HR_Data_Visualization_Dashboard.ipynb`)
This notebook takes the cleaned dataset and translates the statistical findings into an intuitive, business-friendly visual story[cite: 1].
* **Exploratory Data Analysis (EDA):** Mapped out distribution patterns using libraries like `Matplotlib` and `Seaborn`[cite: 1].
* **Visual Dashboards:** Designed stacked bar charts, pie charts, and boxplots to compare employee profiles[cite: 1].

---

## 💡 Key Business Insights
* **Overall Attrition:** The company suffers from a **16.12%** attrition rate, which requires immediate HR intervention[cite: 1].
* **The Overtime Trap:** Employees working overtime face a **30.5%** attrition rate, nearly 3x higher than those who do not (10.4%)[cite: 1]. This relationship was statistically proven with a p-value of 0.0000[cite: 2].
* **High-Risk Roles:** The Sales department is heavily impacted, with the **Sales Representative** role showing an alarming **39.8%** attrition rate[cite: 1].
* **Income & Age Disparities:** The data statistically confirms that younger employees and those with lower average monthly incomes are significantly more likely to leave the company[cite: 1, 2].

---

## 💻 Tech Stack
* **Programming Language:** Python
* **Data Manipulation:** `pandas`, `NumPy`
* **Statistical Analysis:** `SciPy`
* **Data Visualization:** `Matplotlib`, `Seaborn`

---

## 🚀 How to Run the Project
1. Clone this repository to your local machine.
2. Ensure you have the required libraries installed (`pip install pandas numpy scipy matplotlib seaborn`).
3. Run `HR_Data_Cleaning_and_Statistical_Analysis.ipynb` first to process the raw data and generate the cleaned CSV file[cite: 2].
4. Run `HR_Data_Visualization_Dashboard.ipynb` to explore the visualizations and the final HR dashboard[cite: 1].

---
*Created by Eslam Alaa Eldin — Data Analyst & Software Engineer*
