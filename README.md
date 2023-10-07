# Health-Insurance-Claim-Analytics
Introduction
This document presents a statistical analysis of health insurance agency claim data with the goal of gaining insights into claim patterns and trends. The analysis was conducted to inform decision-making processes and improve the efficiency of insurance operations.

Dataset Description
The dataset consists of the following columns:

age: Age of the policyholder(Numeric)
sex: Gender of the policyholder(Categoric)
weight: Weight of the policyholder(Numeric)
bmi: Body Mass Index, a measure of body fat based on height and weight(Numeric)
hereditary_diseases: A policyholder suffering from a hereditary diseases or not(Categoric)
no_of_dependents: Number of dependent persons on the policyholder(Numeric)
smoker: Whether the policyholder is a smoker or non-smoker(1/0)(Catgoric)
city: The city in which the policyholder resides(categoric)
bloodpressure: Blood pressure reading of policyholder(Numeric)
diabetes: Indicates policyholder suffers from diabetes or not (non-diabetic=0, diabetic=1)(Categoric)
regular_ex: A policyholder regularly eexercises or not(no-exercise=0, exercise=1)
job_title: Job profile of the policy holder(Categoric)
claim: The amount claimed by policyholder(Numeric)
Data Size
The dataset consists of 13904 claim records.

Methodology
Data Preparation:
Data cleaning: Removed duplicates and handled missing values. Data transformation: Converted dates to a consistent format.

Exploratory Data Analysis (EDA):
Calculated summary statistics for numerical variables.
Visualized data distribution and claim patterns.
Analyzed claim distribution.
Correlation Analysis:
Performed Pearson's and Spearman's correlation analysis of the data.

Hypothesis Testing:
Conducted a hypothesis test to determine if the mean claim amount is significantly different between gender groups.

Predictive Analytics:
Feature Engineering:

Encoded catgorical features and scaled numerical features. Model Training and Prediction:
Trained different models on the training set and measured the predictive performance of the each model.
Result
Average claim is 13431.81.
Claim tend to increase with age and habits (smoking and non-exercise)
Correlation analysis showed that age and smoking have a strong positive relationship with claim.
Hypothesis test results indicate a significant difference in claim amounts between gender groups (p < 0.05).
Predictive Analytics result show that Random Forest Regressor, XGBoost, Decision Trees and Linear regressors are great for predicting claims.
The most accurate being Random Forest and the least of the models in terms of accuracy is th Linear regression model.
Limitations
The dataset doesn't contain policy ID, year etc., limiting the ability to identify long-term trends.
The analysis assumes the data is representative of the entire insurance population.
External factors, such as changes in healthcare policies, were not considered in the analysis.
Conclusion
This analysis provides valuable insights into health insurance claim data, including claim patterns, average claim amounts, relationship between input features and claim, and the predictability accuracy of future claims.
These findings can inform decision-making processes within the insurance company and help optimize claims processing.
For a more detailed analysis or specific questions, please contact the data analysis team. This is a simplified example, and real-world documentation may include more technical details, additional analyses, and references to code or data sources. The goal is to provide a clear and concise overview of the analysis for both technical and non-technical stakeholders.

Usage
To replicate or build upon this analysis, follow these steps:

Clone this repository to your local machine.
Install the required Python libraries (listed in requirements.txt).
Run the Jupyter Notebook health_insurance_claim_pattern_analysis.ipynb to reproduce the analysis.
Explore the code, visualizations, and comments within the notebook for detailed insights.
Contributing
If you would like to contribute to this project, please follow these guidelines:

Fork the repository. Create a new branch for your feature or bug fix. Make your changes and submit a pull request. Ensure your code follows coding standards and is well-documented. License This project is licensed under the MIT License. Remember to replace the placeholder information with the actual details of your health insurance data analysis project. A well-structured README like this one provides essential information for users, collaborators, and stakeholders who come across your project.
