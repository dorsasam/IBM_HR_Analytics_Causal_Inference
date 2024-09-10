# Causal Inference on Employee Attrition

Using a causal inference approach, this project explores how Job Satisfaction impacts Employee Attrition. We'll walk through steps like data inspection, preprocessing, visualisation, and building a causal model to estimate the effect of job satisfaction on the likelihood of employees leaving a company.

# Project Overview
- Dataset: [IBM HR Analytics Employee Attrition dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- Objective: Estimate the causal effect of Job Satisfaction on Employee Attrition and interpret the results.
- Python Libraries: `pandas`, `scikit-learn`, `seaborn`, `matplotlib`, `dowhy`

# Project Breakdown
1. Data Inspection
We start by loading the dataset and getting a feel for it. We'll check for missing values, understand the data types, and preview basic statistics.
2. Encoding Categorical Features
We convert categorical features like `Department` and `Gender` into numeric values using LabelEncoder to be used in the model.
3. Visualising Feature Correlations
Next, we generate a correlation matrix to see how features relate to each other, especially to the target feature `Attrition`.
4. Identifying Key Features Related to Attrition
We select the features that have the highest correlation (positive or negative) with `Attrition`, helping us focus on the most influential factors.
5. Displaying Feature Distributions
We visualise the distributions of the most relevant features. This gives us an idea of how the values are spread and any potential outliers.
6. Scaling Numeric Features
To prepare the data for modelling, we scale numeric features like `Age`, `MonthlyIncome`, and `YearsAtCompany` so that they are on similar scales.
7. Building the Causal Model
Using DoWhy, we create a causal model to estimate the effect of `JobSatisfaction` on `Attrition`.
8. Simulating an Intervention
We simulate an intervention where `JobSatisfaction` is increased to see how this impacts the attrition rate.

# Results
- Causal Effect of JobSatisfaction on Attrition
  - Estimated Effect: -0.0397
    
    This suggests that for every 1-unit increase in JobSatisfaction, the likelihood of an employee leaving decreases by about 3.97%.
- Simulated Intervention
  - Predicted Attrition Rate: -0.1589
    
    After simulating a significant increase in job satisfaction, the model predicts a drastic reduction in the attrition rate. However, this negative attrition rate is unrealistic, indicating that further model refinements, such as using logistic regression, might be needed.

# Conclusion
This project demonstrates how causal inference can be used to understand relationships between employee satisfaction and attrition. The current model shows that increasing job satisfaction can reduce attrition, but further refinements are needed to get more accurate results.
    
