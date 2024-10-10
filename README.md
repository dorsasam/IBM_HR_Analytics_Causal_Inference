# Causal Inference in HR Analytics Using IBM Dataset
## Project Overview
- Dataset: [IBM HR Analytics Employee Attrition dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
This project utilises causal inference techniques on the IBM HR Analytics dataset to understand the key factors influencing employee attrition. By identifying causal relationships rather than simple correlations, the aim is to make data-driven decisions that lead to actionable HR strategies.

## Tools & Libraries
- Python (`pandas`, `scikit-learn`, `DoWhy`)
- Jupyter Notebook
- Causal Inference with DoWhy Library
  
## Problem Statement
Employee attrition poses significant challenges, such as increased recruitment costs and reduced organisational knowledge. Traditional methods often rely on correlations, which can lead to inaccurate conclusions. This project leverages causal inference to determine the actual causes of employee turnover, allowing HR departments to make effective interventions.

## Methodology
- Data Cleaning & Preparation: Cleaned and prepared the IBM HR dataset by removing missing values and irrelevant columns.
- Exploratory Data Analysis (EDA): Conducted initial analysis to understand key variables, such as job satisfaction and workload.
- Causal Inference: Applied the DoWhy package to establish causal relationships between variables and employee attrition.
- Statistical Testing: Performed hypothesis testing to ensure the robustness of the results.

##Key Results
- Job Satisfaction: Employees with lower job satisfaction are 25% more likely to leave the company.
- Work-Life Balance: Employees who work longer hours show a 15% increase in the risk of attrition.
- Salary: Salary increases had a smaller impact than work-life balance on attrition rates.

## Real-World Applications
These insights assist HR departments in developing targeted strategies, such as improving job satisfaction and work-life balance, to reduce employee turnover. By identifying causal factors, companies can create more effective retention programmes.

## How to Run the Project
- Clone the repository:
bash
```
git clone https://github.com/dorsasam/IBM_HR_Analytics_Causal_Inference.git
```
- Install dependencies:
bash
```
pip install -r requirements.txt
```
- Open the Jupyter Notebook:
bash
```
jupyter notebook HR_Analytics_Causal_Inference.ipynb
```

## Future Improvements
- Explore other confounding variables to refine causal models.
- Expand to other datasets to generalise findings.
- Develop interactive dashboards for better visualisation of causal impacts.
an be used to understand relationships between employee satisfaction and attrition. The current model shows that increasing job satisfaction can reduce attrition, but further refinements are needed to get more accurate results.
