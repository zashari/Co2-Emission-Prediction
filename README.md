# Co2 Emission Prediction: implementing Regression and Classification Model

### Introduction

My project involved creating a comprehensive analysis and prediction model for CO2 emissions based on vehicle specifications. Utilizing a dataset containing various attributes of vehicles, I aimed to understand the factors influencing CO2 emissions and develop both regression and classification models to predict emissions and categorize vehicles based on their emission levels.

### Data Exploration and Preprocessing

#### Initial Exploration
The dataset, "CO2 Emissions_Canada.csv," consisted of 7385 entries with 12 features, including vehicle make, model, engine size, fuel consumption, and CO2 emissions. My initial steps involved:

- Identifying and removing 1103 duplicate entries, resulting in 6282 unique rows.
- Conducting a statistical analysis to understand the distribution of numerical features.
- Generating histograms for each numerical variable and count plots for categorical variables.
- Analyzing the average CO2 emissions per vehicle class.
- Creating a correlation matrix to explore the relationships between different features.

#### Feature Engineering
To prepare the data for modeling, I performed several feature engineering steps:

- Encoding categorical variables such as 'Vehicle Class,' 'Transmission,' and 'Fuel Type' using one-hot encoding.
- Creating interaction features to capture combined effects, like multiplying engine size by the number of cylinders.
- Binning CO2 emissions into categories ('Low', 'Medium', 'High') based on emission levels.
- Standardizing numerical features to have a mean of 0 and a standard deviation of 1.

### Regression Model

#### Model Selection and Training
For the regression task, I selected features influencing CO2 emissions and split the dataset into an 80-20 train-test split. I trained the following models:

- **Decision Tree Regressor:** Achieved an RMSE of 0.067 and R-squared of 0.996.
- **KNN Regressor:** Resulted in an RMSE of 0.112 and R-squared of 0.988.
- **Linear Regression:** Obtained an RMSE of 0.094 and R-squared of 0.991.

### Classification Model

#### Model Preparation
For classification, the target variable was the binned CO2 emission category. The dataset was again split into training and testing sets in an 80-20 ratio.

#### Classifier Training and Evaluation
Several classifiers were trained and evaluated:

- **Decision Tree Classifier:** Achieved an accuracy of 98.33%.
- **Logistic Regression:** Scored an accuracy of 96.74%.
- **KNN Classifier:** Reached an accuracy of 96.82%.
- **Naive Bayes Classifier:** Had a significantly lower accuracy of 45.58%.
- **Random Forest Classifier:** Exhibited the highest accuracy of 98.17%.

### Conclusion

The project successfully demonstrated the application of machine learning techniques in predicting and categorizing CO2 emissions from vehicle data. Decision trees and random forests showed superior performance in both regression and classification tasks. The insights gained from this analysis can be instrumental for policymakers and manufacturers in understanding and reducing vehicle emissions. This project not only allowed me to apply a range of data science skills but also contributed to my knowledge of environmental data analysis.
