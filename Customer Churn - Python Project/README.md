# Customer Churn - Python Project

# 1. Business Insight

Customer churn is a significant challenge for businesses, often leading to lost revenue, diminished market share, and negative impacts on growth and reputation. Customer churn refers to the number of customers who have stopped using a product or service, with the average churn rate being around 30%. While some churn is inevitable, high churn rates can be problematic.

This project aims to explore a customer churn dataset to identify factors contributing to churn and provide insights that can help mitigate the issue. By analyzing patterns in customer behavior, we seek to identify which features are most predictive of churn and offer actionable recommendations for improving customer retention.

# 2. Data Analysis

2.1. Data Understanding
   
The [dataset](https://www.kaggle.com/datasets/muhammadshahidazeem/customer-churn-dataset), retrieved from Kaggle, consists of over 500,000 rows and 12 columns across two files (training and testing datasets). Key features include:

- CustomerID: Unique identifier for each customer.
- Age, Gender, Tenure, Usage Frequency, Support Calls, Payment Delay, Subscription Type, Contract Length, Total Spend: Various customer attributes.
- Churn: Boolean value indicating whether the customer has churned.

2.2. Data Preparation

Steps taken in data preparation:

- Removal of CustomerID: As it serves only as a unique identifier.
- Renaming variables: Spaces in variable names were replaced with underscores for easier referencing.
- Handling missing values: Any null values were removed.
- Binning Age: Age was categorized into intervals (0-20, 21-30, etc.) for easier analysis.
- Encoding categorical variables: Variables such as Gender, Subscription Type, and Contract Length were converted into numerical labels for modeling purposes.

2.3. Exploratory Data Analysis (EDA)

Key Findings from Correlation Analysis:

- The two most correlated features with churn are Total Spend and Support Calls.
- The target variable (Churn) revealed a high churn rate in the dataset.
- Support Calls had the strongest correlation with churn, followed by Total Spend.

Exploratory Insights:

- Customers who make more than five support calls have a significantly higher likelihood of churning.
- Customers who spend more than $500 have a lower likelihood of churning.
- A longer payment delay within the first 20 months leads to higher churn, which decreases after 20 months.
- Age distribution shows that churn is more prevalent among younger customers, with the highest churn rate seen in the 20-30 age group.

# 3. Main Analysis

3.1. Overview of Models

To identify features impacting churn, we used several models:

- Feature Importance Model: To identify the most impactful variables.
- Logistic Regression: To quantify the relationship between key features and churn.
- Decision Tree: To classify churn outcomes based on key variables.
- Random Forest and XGBoost: Used to further improve model accuracy.

3.2. Logistic Regression

Logistic regression was applied using Support Calls and Total Spend as predictors. Key findings:

- Support Calls: A strong positive correlation with churn, with every additional support call increasing churn likelihood.
- Total Spend: A negative correlation, where higher spending reduces the likelihood of churn.
- Both features were statistically significant, with very low p-values.

3.3. Decision Tree

The decision tree classified churn outcomes based on the most impactful variables. Model performance metrics:

- Accuracy: 88.71%
- Precision: 87.44%
- Recall: 93.07%
- F1 Score: 90.17%
- AUC: 88.16%

The model effectively predicts customer churn, providing a foundation for intervention strategies.

3.4. Random Forest and XGBoost

Both models achieved high accuracy and F1-scores around 93%, further confirming the robustness of the analysis.

3.5. Clustering

Using Usage Frequency, Support Calls, Tenure, Payment Delay, and Total Spend, we applied clustering techniques, identifying three distinct customer groups for further segmentation and targeting.

# 4. Recommendations

4.1. Personalized Support

We recommend a focus on personalized customer support, particularly for customers who make frequent support calls. Key strategies include:

- Analyzing support data: Identify common issues and recurring challenges.
- Implementing tiered support systems: Prioritize customers with complex issues to reduce churn risk.
- Proactive engagement: Reach out to customers showing signs of dissatisfaction early to offer tailored solutions.

4.2. Increase in Customer Retention

Develop customer loyalty programs that go beyond basic transactions. By analyzing churn data and personalizing rewards based on customer profiles, companies can enhance loyalty and create stronger connections with customers.

# Conclusion

By understanding the factors driving customer churn, businesses can take targeted actions to improve customer retention. This project provides actionable insights and models that help predict churn and offer a roadmap for reducing it through personalized support and strategic engagement.
