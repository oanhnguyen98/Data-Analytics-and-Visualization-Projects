# Salary and Job Satisfaction Prediction - R Project

# Project Overview

This project explores the relationships between various factors like age, company size, revenue, skills, job satisfaction, and salary in the data science and data analytics industry. Using data sourced from Kaggle’s [Salary Prediction](https://www.kaggle.com/datasets/thedevastator/jobs-dataset-from-glassdoor/data) dataset, we aim to uncover insights that will help stakeholders - such as recruiters, finance departments, executives, and job seekers - make data-driven decisions. The analysis serves as a toolkit to understand salary expectations, improve employee retention, and enhance workplace satisfaction. Ultimately, the project develops predictive models to estimate salary and job satisfaction based on specific inputs.

# 1. Dataset

The dataset used is "eda_data.csv", which contains 33 variables and 742 rows. This data includes:

- Demographics: Age, job seniority, and job title
- Company Information: Company size, revenue, and ownership type
- Job Satisfaction: Ratings from employees (0–5 scale)
- Salary Information: Minimum, maximum, and estimated average salary
- Skills: Whether the job requires knowledge of Python, R, AWS, Spark, and Excel

The data was preprocessed to address missing values and outliers, convert salary from hourly to annual where applicable, and create usable variables for modeling.

# 2. Exploratory Data Analysis (EDA)

Key findings from the exploratory data analysis include:

- Age and Salary: No clear relationship was observed between age and salary.
- Salary and Company Size: Small companies tend to pay higher median salaries compared to large and medium-sized companies.
- Job Satisfaction and Salary: Satisfied employees tend to earn higher median salaries than neutral or very satisfied employees, although variability exists.
- Job Title and Salary: Directors earn the highest median salary, followed by R&D engineers and machine learning engineers.
- Job Satisfaction by Company Size: More employees in small companies are "very satisfied" compared to medium and large companies.
- Skills and Salary by State: Python, Excel, and Spark are the most in-demand skills across the top-paying states (CA, MA, IL, NJ, and DC).

# 3. Main Models

3.1. Salary Prediction Models

We built the following models to predict average salary:

- Multiple Linear Regression
- Random Forest
- Gradient Boosting
- XGBoost

Best Model: The Random Forest model performed best with an R² score of 0.54. However, all models had relatively low predictive power due to the limited size of the dataset.

3.2. Job Satisfaction Prediction Models

We built models to classify job satisfaction:

- Random Forest
- Extreme Gradient Boosting
- Naive Bayes
- Gaussian Naive Bayes
- Best Model: Random Forest also performed best in classifying job satisfaction.

3.3. N-Way ANOVA

We conducted an N-Way ANOVA to test how various factors (job title, seniority, skills) and their interactions impact salary. Key findings include:

- Job title, seniority, Python skill, and Spark skill have significant effects on salary.
- There are significant interaction effects, such as between job title and Python skill, and job seniority and Python skill.

# 4. Recommendations

For Recruiters:
- Use insights to set realistic salary benchmarks and attract top talent.
- Focus on recruiting for specific skill sets, like Python and Excel, which are highly valued across all states.

For Finance Departments & Executives:
- Reevaluate salary structures to ensure competitiveness, especially for companies with smaller revenues.
- Develop a flexible budgeting strategy that takes into account job satisfaction and market demand for certain skills.

For Job Seekers:
- Use insights to understand your market value and negotiate accordingly.
- Focus on developing in-demand skills like Python, Excel, and Spark to enhance earning potential.

# 5. Future Directions

- Expand the Dataset: Larger datasets could provide more accurate predictions and help uncover trends not visible in smaller samples.
- Add Additional Features: Incorporating variables like education level, years of experience, and detailed skills may offer deeper insights into salary determinants.
- Salary Prediction Tool: Consider developing a user-friendly tool that allows job seekers and employers to predict salary ranges based on input factors like job title, company size, and skills.
- Explore Remote Work Impact: As remote work becomes more prevalent, future analyses could explore how it affects salary structures and job satisfaction.

# 6. Limitations

- Small Dataset: Only 742 rows, limiting the accuracy of predictive models.
- Limited Features: Important factors such as years of experience and education level are not included in the dataset.
# Conclusion

This project provides valuable insights into salary and job satisfaction dynamics for data analysts and scientists, offering a foundation for both individual career growth and organizational strategy. While the Random Forest model performed best, expanding the dataset and incorporating more features could further enhance predictive accuracy. The analysis has implications for stakeholders ranging from job seekers to organizational leaders looking to optimize compensation strategies.
