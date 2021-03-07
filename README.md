# Project 2 - Ames Housing Data and Kaggle Challenge

This project aims to provide main features of a house that affects its price, done by doing Regression models.

### Data Dictionary:
http://jse.amstat.org/v19n3/decock/DataDocumentation.txt

Dealing with missing values in data:
For this project, both datasets have missing value columns have not been deleted, rather it has filled with No, None or 0 instead so that we can create a correlation for each variable.

### Methodology:

Dealing with missing values in data:
For this project, both datasets have missing value columns have not been deleted, rather it has filled with No, None or 0 instead so that we can create a correlation for each variable.

1. Create a correlation between all numeric features first and analyze.
2. Create a scatter plot to see the relationship between numeric features with the sale price.
3. Seek to see out outlier by conducting boxplot and filtering the outliers out.
4. Analyze if removing outliers improved the correlation.
5. Conduct outside research to see important categorical features that affect sale price.
6. Include finding from research by applying it to the model.
7. Conduct a boxplot of categorical features to see if there is a trend that some features are more sensitive than others.
8. Separate categorical features into ordinal features and nominal features.
9. Map values into categorical features that are ordinal and analyze how it has impacted the model.
10. Analyze each nominal feature one by one to see if it impacts sale price.
11. For features that seem to have an impact, create dummy variables and add it to the model.
- if the model error reduces, it means the categorical variable added to the model is good. Therefore, keep it in the model.
- if the model error increases, it means the categorical variable added to the model is not good. Therefore, remove it.
12. Continue repeating steps 10 and 11 for all nominal features.
13. Using lasso regression, remove insignificant features.

### Analysis:
- Remove insignificant features did not affect the model.
- Proceeded to removing features that affect the price by at least 500 dollars. This increase the error of the model, but not by much.
- Proceeded to removing features that affect the price by at least 1000 dollars. Even this increase the error of the model, however, its validation score and error still remained good.

Therefore, ending up with a total of 36 features.

### Conclusion:
Top 10 Factors increasing the price of a house are:
1. Ground Liv Area
2. Overall Quality
3. Basement square feet type 1 that is finished
4. Year Built
5. Neighborhood - Northridge Heights
6. Masonry veneer area in square feet
7. Total Basement square feet
8. Neighborhood - Stone Brook
9. External Quality
10. Overall Condition

- As per top 10 factors increasing the price of a house, general look and feel of the house seems to be an important factor.
- The total livable surface area of the house also plays an important factor.
- Being in certain neighborhood would certainly yield a higher price.

Top 10 Factors reducing the price of a house are:
1. MS Sub Class
2. Masonry veneer type - Brick Face
3. Bedroom above grade
4. Basement Condition
5. Roof Style - Mansard
6. Masonry veneer type - Brick Common
7. Kitchen above grade
8. Primary Exterior covering the house - Hard Board
9. Sale Type - Court Officer Deed/Estate
10. More than 1 type of garage

- The type of dwelling has quite a significant impact on house price
- Detail inspection aspect such as roof style, masonry veneer type and primary exterior plays down the price.
