# SC1015 Mini Project - Prediction of Laptop Price

## Repository Description
This repository is submitted to Nanyang Technological University as part of a graded assignment for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on [Laptop sales price prediction 2024](https://www.kaggle.com/datasets/siddiquifaiznaeem/laptop-sales-price-prediction-dataset-2024).

## Dataset Used
Our dataset is from Kaggle: "Laptop sales price prediction 2024" by Siddiqui Faiz Naeem\
Source: https://www.kaggle.com/datasets/siddiquifaiznaeem/laptop-sales-price-prediction-dataset-2024

This dataset contains information about various laptops, including specifications and prices, curated for sales price prediction. With features ranging from processor details to display specifications, this dataset serves as a valuable resource for analyzing trends and predicting laptop prices.

## Table of Contents:
1. Problem Formulation
2. Data Preparation and Cleaning
3. Exploratory Data Analysis
4. Machine Learning
5. Data-Driven Insights and Conclusion
6. References

### 1. Problem Formulation
* How do different factors affect the price of laptop?
* Which model would be the best to predict laptop price?

### 2. Data Preparation and Cleaning
In this section of the project, we prepped and cleaned the dataset to help us analyze our data better and also to help us use our data for the purposes of machine learning in the later sections.  
We performed the following:  
**Preliminary Feature Selection:** 22 variables out of 26 were selected.  
**Dropping NaNs:** All the rows containing NaN values were dropped.  
**Currency Changing:** Convert the currency from INR to SGD  


### 3. Exploratory Data Analysis
Then, we explored our data frames further using Exploratory Data Analysis to explore the relationship between variables and decide which predictors to use.
**Exploring Response Variable `Price`:** Median of around $1027 was seen. Data is positively skewed.
**Exploring Numerical Variable:** 3 numeric variables with higher correlation with `Price` were chosen to be the predictors.
**Exploring Categorical Variable:** 3 categorical variables were chosen to be the predictors.
**Encoding Categorical Variables:** The categorical variables in both the DataFrames were encoded appropriately.

### 4. Machine Learning
1. **Linear Regression**
2. **Random Forest**
3. **Voting Regressor**

### 5. Data-Driven Insights & Conclusion
From our analysis, we found that for the numerical predictors we have used, RAM size, storage capacity, and Vertical Pixel Resolution all have a strong positive correlation with price compared to other predictors.

For categorical, laptops with SSD have a larger median price than laptops with hard disks. Intel CPUs also have a higher median price than AMD CPUs while Touch Screen laptops also have a higher median price than laptops without touch screens. This can imply that these factors have a bigger influence on price than their counterparts.

Overall, the predictors above have a big influence on price and could be due to consumers thinking that a better laptop is a laptop with one that includes these factors inside.

For our second problem definition, from our analysis, we see that the random forest model gives us the highest explained variance and lowest mean square error. As it has the highest prediction accuracy from this analysis, we believe the random forest model to be the best model in predicting laptop price.

### 6. Reference
1. S. Naeem, “Laptop sales price prediction 2024,” Kaggle. https://www.kaggle.com/datasets/siddiquifaiznaeem/laptop-sales-price-prediction-dataset-2024
2. A. Jayant, “Forecasting Laptop Costs: A Machine Learning Approach,” Medium, Nov. 24, 2023. https://medium.com/@aniketjayant953/forecasting-laptop-costs-a-machine-learning-approach-3dbcf9bbf5c6.
3. “Laptop-Price-Prediction/model/model.ipynb at main · LuluW8071/Laptop-Price-Prediction,” GitHub. https://github.com/LuluW8071/Laptop-Price-Prediction/blob/main/model/model.ipynb.
4. E. R. Sruthi, “Random Forest | Introduction to Random Forest Algorithm,” Analytics Vidhya, Jun. 17, 2021. https://www.analyticsvidhya.com/blog/2021/06/understanding-random-forest/
5. “Voting Regressor,” GeeksforGeeks, Oct. 25, 2023. https://www.geeksforgeeks.org/voting-regressor/
6. “Python Machine Learning Multiple Regression,” www.w3schools.com. https://www.w3schools.com/python/python_ml_multiple_regression.asp
7. D. Yadav, “Categorical encoding using Label-Encoding and One-Hot-Encoder,” Medium, Dec. 09, 2019. https://towardsdatascience.com/categorical-encoding-using-label-encoding-and-one-hot-encoder-911ef77fb5bd
8. “Folium — Folium 0.1.dev1+g57e8eae documentation,” python-visualization.github.io. https://python-visualization.github.io/folium/latest/

## Contributors
School of Computer Science and Engineering, NTU Singapore\
AY2023/24 SC1015 ECDS1 Group 5

* GABRIELLA SIAOMAN GABR0031@E.NTU.EDU.SG
    (EDA Categorical Variable, Linear Regression)
* TAY JIAN YUAN JTAY090@E.NTU.EDU.SG
    (Data Cleaning and Preparation, Voting Regressor, Price Predictor)
* LAI LI SONG LLAI005@E.NTU.EDU.SG
    (EDA Numerical Variables, Random Forest)
