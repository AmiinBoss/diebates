# diebates
Diabetes Dataset Analysis


Overview
This project presents an end-to-end data analysis and visualization of the Kaggle Diabetes Dataset, widely used for machine learning and health informatics tasks. The analysis focuses on uncovering the relationships between key health indicators and the presence of diabetes, using modern data cleaning techniques and insightful visualizations to answer relevant research questions about risk factors and demographic patterns.

Dataset Description
The Diabetes Dataset contains the following variables:

Pregnancies: Number of times pregnant

Glucose: Plasma glucose concentration (2 hours in an oral glucose tolerance test)

BloodPressure: Diastolic blood pressure (mm Hg)

SkinThickness: Triceps skin fold thickness (mm)

Insulin: 2-hour serum insulin (mu U/ml)

BMI: Body mass index (weight in kg/(height in m)^2)

DiabetesPedigreeFunction: Diabetes likelihood score based on family history

Age: Age in years

Outcome: Diabetes status (1 = diabetic, 0 = non-diabetic)

Source: Kaggle, provided by user "mathchi".

Research Questions
Risk Factor Analysis:
What are the most significant risk factors associated with diabetes in the dataset?

Feature Relationships:
How do features such as glucose, BMI, and age interact, and how do these relationships differ between diabetic and non-diabetic individuals?

Demographic Analysis:
Are there age-related or other demographic patterns in the prevalence of diabetes?

Data Cleaning Process
Ensuring data quality was a critical step in this analysis:

Identification of Invalid Values:
Placeholder zeros were detected in five key columns (BMI, BloodPressure, Glucose, SkinThickness, Insulin). Since zero is physiologically implausible for these variables, they were treated as missing values.

Imputation Strategy:

Median Imputation: For columns with relatively few zeros (BMI, BloodPressure, Glucose), missing values were replaced with the median.

Predictive Mean Matching: For columns with many missing values (SkinThickness, Insulin), the mice package was used for imputation, ensuring realistic values and minimizing bias.

Post-Cleaning Validation:
The dataset was validated to ensure no implausible zeros remained and that data integrity was maintained.

Analysis & Visualizations
A variety of visualizations were created to answer the research questions, including:

Distribution Plots:

Glucose Levels: Clear separation, with diabetics showing right-skewed distributions at higher glucose levels.

BMI: Diabetics tend to have higher BMI, though there is significant overlap with non-diabetics.

Scatter Plots & Pairs Plot:

Relationships among glucose, BMI, and age were explored, showing strong correlation between BMI and glucose (especially in non-diabetics), but weak correlation between age and either metric.

Density and Proportion Plots by Age:

Analysis of the age distribution revealed that while diabetes prevalence increases with age (notably after 70), the condition is present across all age groups.

Key Findings
Glucose and BMI are the strongest indicators of diabetes status in this dataset.

Age is a moderate risk factor, especially in older populations, but not a clear-cut predictor by itself.

There is no single variable that fully separates diabetic from non-diabetic individuals; rather, diabetes risk is driven by a combination of factors.

Data cleaning (handling zeros as missing) was crucial for reliable results, using appropriate imputation methods for different variable types.

Conclusion
This project demonstrates a full data science pipeline—from cleaning and preprocessing, through exploration and visualization, to statistical analysis—on a real-world medical dataset. The findings reinforce established medical knowledge while highlighting the complexity of diabetes risk factors and the importance of clean, well-prepared data.

Getting Started
Download the dataset from Kaggle.

Review the Jupyter notebooks/scripts provided for step-by-step analysis.

Visualizations and results can be reproduced using the provided code.

Contact
For questions, collaborations, or suggestions, please open an issue or contact shaam via https://www.linkedin.com/in/mohamed-abdullahi-kasim-12b9a732a/ .

