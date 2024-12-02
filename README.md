# Analyzing the Effect of Weather and Income on IQ Across Countries

## Introduction
In this project, we aim to explore how **weather (temperature)** and **average income** influence the **IQ levels** of countries worldwide. By analyzing data from various countries, we used regression models to understand the relationships between these factors.

## Data Overview
The dataset used contains information about the following variables:
- **Rank**: The country's rank based on IQ levels.
- **Country**: The name of the country.
- **IQ**: The average IQ level of the population in each country.
- **Average Temperature (avg_temp)**: The average temperature in the country.
- **Average Income (avg_income)**: The average annual income in the country.
- **Education Expenditure (education_expenditure)**: The amount spent on education as a percentage of GDP.

## Methodology
We used **multiple linear regression** and **polynomial regression** to explore the relationships between **IQ**, **average temperature**, and **average income**. Initially, a simple linear regression was applied to see the effects of income on IQ. However, the relationship between temperature and income was analyzed through a polynomial regression model.

Key steps:
1. **Data Preprocessing**: Cleaned the dataset by handling missing values and ensuring the data was in the correct format.
2. **Exploratory Data Analysis (EDA)**: Visualized relationships between variables through scatter plots and histograms.
3. **Regression Models**: 
   - Performed **simple linear regression** using only **average income**.
   - Implemented **multiple regression** using both **average temperature** and **average income**.
   - Applied **polynomial regression** to model non-linear relationships.
4. **Model Evaluation**: Used **R-squared** to evaluate how well the models explained the variation in IQ levels.

## Results
- The simple linear regression model suggested that **income** alone had a minimal effect on IQ.
- A **polynomial regression** model with **average income** improved the model fit, but the R-squared value was moderate, indicating that income alone did not fully explain IQ variation.
- A **multiple regression** model with both **temperature** and **income** showed a moderate correlation, but temperature had a stronger influence on IQ.

The **R-squared values**:
- Simple Linear Regression: **R² = 0.4028** (for income).
- Polynomial Regression: **R² = 0.4543**.
- Multiple Regression (with both temperature and income): **R² = 0.5108**.

## Conclusion
Based on the analysis, **temperature** was a stronger predictor of IQ than **income**, although both factors did contribute to explaining the variance in IQ levels. The results suggest that environmental factors, like temperature, may play a more significant role in shaping IQ scores globally than economic factors like income.

## Next Steps
To improve the model:
- Consider incorporating additional features, such as **education expenditure** or **healthcare spending**.
- Explore more complex models, such as **non-linear regression** or **machine learning** techniques, to capture more intricate relationships.
