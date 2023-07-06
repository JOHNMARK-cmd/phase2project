# phase2project
# OVERVIEW
# INTRODUCTION
The real estate agency operating in Northwestern county wants to an analysis on the types of houses in the county to asses their value. However they lack knowledge on what types of houses to choose and the price the range in order to make firm decisions that will generate profits.
# Business understanding and Data understanding
 # The stakeholder
The real estate agency lacks enough knowledge on how to perform best in this field. The business problem is to develop a predictive model that can accurately estimate house prices based on various features provided in the King County House Sales dataset. The agency aims to use this model to guide their clients in setting competitive prices for their properties, optimize their marketing strategies, and improve their overall business performance in the real estate market.
# Project goal
To develop a predictive model that can accurately estimate house prices that is profit yielding in various features such as location, size, condition, and amenities.

# Data understanding
To achieve this, we will build multiple models starting with a basic model and then iteratively refining it to improve predictive accuracy and interpretability. By analyzing the dataset, performing data visualization, and evaluating different model performance, we can gain insights into the key factors influencing house prices in the area and provide actionable recommendations to the real estate agency.

# Methods
The size of the dataset is wide allowing for a robust analysis and provides a comprehensive view of the houses' information. I will perform a statistical data analysis using varous data science modeling analytical tool and come up with visualizations that can describe the data better to the stakeholders. This will help identify key trends and characteristics of the houses such as location, size, condition, and amenities.

However, it is important to acknowledge that the datasets may have some limitations. They might not capture the entire universe of houses, and there could be missing or incomplete data for certain houses. Additionally, the data might be subject to biases or limitations inherent in the sources themselves. Despite these limitations, the datasets provide valuable insights into the movie industry and are suitable for addressing the business problem at hand.
# Conclusion
The aim of this project is to provide valuable insights for the real estate agency through exploring the dataset. Through this comprehensive house dataset analysis, I can identify the types of houses to focus on. The findings of this analysis will enable stakeholders to make informed decisions concerning the types of houses to invest on. Through these insights, the real estate agency can become successful in the real estate industry and establish a strong presence as a best genuine business people.

## DATA PREPARATION AND DATA ANALYSIS
# Data preparation
Here, I used the dataset from kc_house_data. This data provides a wide range of data collected overtime that can be a good starting point.

# Rationale of the analysis: 
We are using statistical analyses, specifically multiple linear regression modeling, to capture the relationships between the independent variables and the dependent variable in a quantitative manner. Regression coefficients provide us with the magnitudes and directions of these relationships, enabling us to estimate the impact of each feature on house prices. Using regression coefficients goes beyond the visual exploration of data and provides precise numerical measures of the feature contributions.

The problem of analyzing house sales in a northwestern county is suitable for multiple linear regression because it involves multiple independent variables that may collectively influence the house prices. This form of analysis allows us to estimate the relative importance of each feature and understand how changes in these features affect the predicted house prices.

# Limitations of the analysis: 
The assumptions of linear regression: such as linearity, independence, homoscedasticity, and normally distributed errors. Violations of these assumptions can affect the validity of the model. The presence of multicollinearity (high correlation among independent variables) can lead to unstable coefficient estimates. Missing data and outliers should also be considered.

Missing Data: Missing data handling is crucial but not explicitly addressed in this analysis. Dropping missing values might lead to a loss of information, and imputation techniques could be explored.
# Data analysis process
Here, I will use linear regression modeling in analysing the dataset. I will perform data exploration na d cleaning on the data, bulid a baseline model, iterate through it and report on its metrics. Then use visualizations and finally come up with recommendations on the findings of the analysis.
# Modeling
Building baseline model
Iterating though the model
# Regression results
1. Interpreting one-hot encoded results
The model is overally statistically significant with F-statistic of about 96%. Which is seemingly good.

The r-squared and the adjusted r-squared coefficients are fairly the same. This means that out model explains about 65% of the variance price.

However the r-suared has some limitations in that as we add more prdictors the r-squared only goes to increase.

The const means that variables are 1.

2. Interpreting baseline model results
The model is statistically significant overall, with F-statistic and p-value of well above 0.05.

The model explains about 96% of the variance in price. This might be good.

Each time the reference category changes, the const and the other coefficients change. Const changes because it represents the value when all predictors are 0, and this means that const represents when the reference category is true.

The model coefficients are oveally statistically significant with t-statistic p-value well above 0.05.

3. Interpreting iterated model results.
The model's r-squared and adjusted r-squared are generally statistically significant, with p-values of about 0.05.
Each time the reference category changes, the const and the other coefficients change. Const changes because it represents the value when all predictors are 0, and this means that const represents when the reference category is true.
For each increase in the model coefficients (sqft_living, bedrooms, bathrooms, floors) there is an associated increse in price of houses.

4. Final model results
Based on the small p-values, we can say that the model is statistically significant.
The baseline r-squared explain about 51% of variance in price while the iterated model explains a little more improved r-squared of about 56% of the variance on the price.

The model feature coefficients are overally statistically significant, with t-statistic p-values well above 0.05.

However its important to note that the r-squared has limitations associated with it such as when we add more predictors, the r-squared is going to increase. This could be addressed with error-based metric but the two peform better in differnt cases.

# Recommendations: 
Based on the model results and limitations, the real estate agency should consider the following actions:

1. The real estste agency should use the model as a tool to estimate house prices accurately, guide pricing strategies, and make informed business decisions.

2. The coefficient values can guide the real estste agency in understanding the relative importance of each feature on house prices. For example, a positive coefficient indicates an increase in price with an increase in the corresponding feature, while a negative coefficient indicates a decrease in price.

3. The real estate agency should be aware of the limitations and uncertainties in the analysis, considering potential model assumptions and the excluded factors that could impact house prices. They should use the models as a supportive tool alongside domain knowledge and market expertise.

By leveraging the multiple linear regression models, stakeholders can make more accurate price estimations and gain valuable insights into the factors driving house prices in the Northwestern county.
