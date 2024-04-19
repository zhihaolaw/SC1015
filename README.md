# SC1015 Life_Expectancy_prediction

## About  Life_Expectancy Dataset

## Context
Although there have been lot of studies undertaken in the past on factors affecting life expectancy considering demographic variables, income composition and mortality rates.  In a nutshell, this study will focus on immunization factors, mortality factors, economic factors, social factors and other health related factors as well. Since the observations this dataset are based on different countries, it will be easier for a country to determine the predicting factor which is contributing to lower value of life expectancy. This will help in suggesting a country which area should be given importance in order to efficiently improve the life expectancy of its population.

## Content
The project relies on accuracy of data. The Global Health Observatory (GHO) data repository under World Health Organization (WHO) keeps track of the health status as well as many other related factors for all countries The data-sets are made available to public for the purpose of health data analysis. The data-set related to life expectancy, health factors for 193 countries has been collected from the same WHO data repository website and its corresponding economic data was collected from United Nation website. Among all categories of health-related factors only those critical factors were chosen which are more representative. It has been observed that in the past 15 years , there has been a huge development in health sector resulting in improvement of human mortality rates especially in the developing nations in comparison to the past 30 years. All predicting variables was then divided into several broad categories:​Immunization related factors, Mortality factors, Economical factors and Social factors.

## Acknowledgements
The data was collected from WHO and United Nations website with the help of Deeksha Russell and Duan Wang.

## About
This is the mini project for *NTU-SC1015 Tutorial Group FCE3, Group 3 (Introduction to Data Science and Artificial Intelligence)* .
Singapore ranks as 6th blue zone having one of the highest longevigity age, hence it is crucial for us to explore into factor that affect the life expectancy in the world. In this project, our group's main focus is to analyse the relationship between life expectancy and top 3 variables/factors. The approaches includes/involves both predictive modelling and clustering methods. Predictive modelling helps us predict life expectancy based on the top 3 variables we have chosen based on the correlation plot. In addition to that, clustering helps us identify groups within the expectancy data based on the various factors, helping us further understand about patterns regarding life expectancy. By combining these methods, we aim to get better understanding about the factors that affect life expectancy.

## Problem definition
1. Which of the variables is the best in terms of predicting life expectancy?
2. Which model would be the best in helping us to predict the life expectancy?

## Dataset used
The dataset used for this project is retrieved from [here](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data)

For the cleaned dataset, please download it from [here](https://github.com/zhihaolaw/SC1015/blob/main/cleaned_life_expectancy_data.csv)
For the EDA python notebook, please view at [here](https://github.com/zhihaolaw/SC1015/blob/main/SC1015_mini_project_EDA_cleaned_data.ipynb)

## Presentation
Link to the presentation video from the submission.

## Brief process walkthrough

**[Data Preparation & Cleaning]**
   1. Rename Columns of Dataframe
   2. Data Extraction
   3. KNNImputer for Replace Null Value
   4. SelectKbest
   5. Replace Outlier with Mean Value

**[Exploratory Data Analysis]**
   1. Bi-variante Analysis and Visualization
   2. Uni-variante Analysis and Visualization
   
**[Machine Learning Model]**
   1. Linear Regression
   2. Support Vector Regression
   3. Random Forest Regression
   4. K-Means Clustering
   5. Decision Trees

+ The code in the python notebook is used for Regression Analysis to predict Life Expectancy using the 3 different predictor variables. This includes, Linear Regression, SVR, Random Forest Regression. Each Model's performance is judged based on the metrics like Explained Variance (R^2) and Mean Squared Error (MSE) on both training and testing datasets.

+ The code in the python notebook, we used K-means clustering to group countries based on the factors, determining the amount of clusters with the Elbow Method. In addition to that, we used Principal Component Analysis (PCA)  to visualise the data so that we can inspect how well the countries are separated based on the factors.

+ The Decision Tree classification was first used to compare the importance of the 3 different predictor variables which are Income, Schooling and Adult Mortality and classify our data according to them. The classification trees were  also modelled after each variable separately, and their performance is judged based on the metrics like accuracy, True Positive Rate (TPR) and False Positive Rate (FPR) on both training and testing datasets.


## Conclusion
1. Income was the best variable in predicting the life expectancy of a person. 
2. People who live in countries with a higher GDP per capita often have a higher average lifespan
3. Important for our economy to remain vibrant and inclusive as it directly impacts the health and longevity of our population
4. Schooling translates into access to quality education
5. Education not only enhances individual health literacy but also fosters healthier lifestyle choices
6. Adult mortality is dependent on factors like healthcare accessibility, disease prevalence, and lifestyle factors

## Key learning points
1. Concepts about KNNInputer, KBest Feature
2. Concepts about Support Vector Regression
3. Concepts about Random Forest Regression
4. Concepts about K-Means Clustering
5. Collaborating using Github

## Contributors
1. Justin (Data Extraction, Decision Trees)
2. @zhihaolaw (Data Preperation & Cleaning, Exploratory Data Analysis)
3. Rahul (Linear Regression, Support Vector Regression, Random Forest Regression, K-Means Clustering)

## References
1. https://scikit-learn.org/stable/modules/generated/sklearn.impute.KNNImputer.html
2. https://neuraldatascience.io/5-eda/data_cleaning.html
3. https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data
4. https://www.worldometers.info/demographics/life-expectancy/
5. https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html
6. https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html
7. https://scikit-learn.org/stable/modules/clustering.html
8. https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html
9. https://www.analyticsvidhya.com/blog/2020/03/support-vector-regression-tutorial-for-machine-learning/
10. https://www.geeksforgeeks.org/pandas-cut-continuous-to-categorical/


