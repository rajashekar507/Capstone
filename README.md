# UNDERSTANDING AND PREDICTING CUSTOMER DEPOSITS: A DATA-DRIVEN ANALYSIS PROPOSAL

**Author:** Rajashekar Reddy Muskula  
**Course:** BAN 586 Capstone Project, Spring 2025

---

## Table of Contents
1. [Executive Summary](#executive-summary)
2. [Project Statement](#project-statement)
3. [Data and Methods](#data-and-methods)
    - [Data](#data)
    - [Methods](#methods)
4. [Model and Analysis](#model-and-analysis)
    - [Model](#model)
    - [Analysis](#analysis)
5. [Validation and Testing](#validation-and-testing)
    - [Validation](#validation)
    - [Testing](#testing)
    - [Cross Validation](#cross-validation)
6. [Results and Recommendations](#results-and-recommendations)
    - [Results](#results)
    - [Recommendations](#recommendations)
7. [Conclusion](#conclusion)
8. [Acknowledgements](#acknowledgements)
9. [References](#references)
10. [Repository Structure](#repository-structure)

---

## 1. Executive Summary
The analysis uses 2022 customer data to determine which factors affect Foothill Bank's deposit growth. Foothill Bank contains vast historical customer data, yet had no established approach to determine why customers boost their deposits. The analysis of customer demographic information alongside behavioral patterns and economic environments will help establish strategies for attracting more depositors to the bank.

Key findings include:
- Higher deposits are associated with married clients, higher income, moderate expenditure, and low-poverty areas.
- Contacting clients via mobile phone in May yields the highest probability of deposit increases.
- Predictive models (Logistic Regression, Linear Regression, Random Forest) were used to identify and validate these drivers.

---

## 2. Project Statement
This project uses 2022 client data to identify what drives Foothill Bank's deposit growth. The bank possesses rich historical data but lacks a systematic, data-driven methodology to recognize behavioral patterns or identify the customers who will increase their deposit amounts. Advanced analytics is the main technique used in this project to identify important demographic, behavioral, and economic elements that impact deposit growth.

---

## 3. Data and Methods
### 3.1 Data
- Customer demographics: age, job, marital status, education, credit default, housing loan, contact type, interaction month/day, duration, campaign details, previous outcomes.
- Macroeconomic variables: employment variation, consumer price/confidence index, 3-month Euribor, number of employees.
- Supplementary data: average poverty rate, annual household expenditure, annual median income (see references).
- Target variable: "y" (deposit subscription).

### 3.2 Methods
- **Excel:** Data cleaning, initial exploratory analysis.
- **Tableau:** Interactive dashboards and visualizations.
- **Python:** Advanced analysis and predictive modeling (Pandas, Scikit-learn).
- **RapidMiner:** Machine learning (Random Forest) for non-linear pattern detection.

---

## 4. Model and Analysis
### 4.1 Model
- **Logistic Regression:** Predicted deposit subscription using categorical/continuous variables. Achieved 99% accuracy for certain segments.
- **Linear Regression:** Modeled deposit amounts using age, income, expenditure, contact method, and poverty rate. Achieved 89.06% accuracy.
- **Random Forest (RapidMiner):** Identified key non-linear relationships and variable importance.

### 4.2 Analysis
- May had the highest deposit conversions; December the lowest.
- Cellular contact method outperformed traditional telephone.
- Married clients, higher income, moderate spenders, and those in low-poverty areas are most likely to increase deposits.
- See `/docs` for full report and `/dashboards` for Tableau dashboard.

---

## 5. Validation and Testing
### 5.1 Validation
- Hypothesis tests (t-tests) on call durations by marital status.
- Correlation analysis between poverty, income, expenditure, and deposit growth.

### 5.2 Testing
- Multiple models evaluated; Logistic Regression achieved 99% accuracy for call duration/marital status.
- Linear Regression used for broader demographic/economic prediction (89.06% accuracy).
- Random Forest confirmed key drivers.

### 5.3 Cross Validation
- Data split into training/testing sets.
- Models validated for overfitting and reliability.

---

## 6. Results and Recommendations
### 6.1 Results
- Lower poverty, higher income, and moderate expenditure drive deposit growth.
- Married clients and those without personal loans are most likely to increase deposits.
- May and cellular contact methods are optimal for outreach.
- Predictive models provide actionable segmentation for marketing.

### 6.2 Recommendations
- Target married, higher-income, moderate-spending clients in low-poverty areas.
- Focus marketing in May and use cellular contact methods.
- Continuously update predictive models with new data.
- Tailor service packages to client economic conditions.

---

## 7. Conclusion
This project provides Foothill Bank with a data-driven framework to increase deposit subscriptions. By leveraging demographic, behavioral, and economic insights, and deploying predictive models, the bank can optimize marketing and engagement strategies for sustainable growth.

---

## 8. Acknowledgements
- Kristin Marie Greenwalt: Capstone guidance and feedback
- Sumana Talusani: Tableau and data visualization support
- Satya Sai Sugandam: Python, hypothesis testing, and report creation
- BCC: Presentation and report support

---

## 9. References
- Bank Data: Foothills Bank 2022
- Average Poverty Data: [Welfare Info](https://www.welfareinfo.org/poverty-rate/arizona/)
- Median Income, Annual Household Expenses: [Statista](https://www.statista.com/statistics/233184/median-household-income-in-the-united-states-by-age/)

---

## 10. Repository Structure
```
/docs
  - BAN586 Final Report Muskula.docx
  - Rajashekar Reddy Final Presentation.pdf
/dashboards
  - Final Capstone Dashboard.twbx
README.md
```
- `/docs`: Reports and presentations
- `/dashboards`: Tableau dashboard
- `README.md`: Project overview and instructions

---

For questions or collaboration, please contact **Rajashekar Reddy Muskula** via GitHub. 