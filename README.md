# SC1015 Life_Expectancy_prediction

## About  Life_Expectancy Dataset

## Context
Although there have been lot of studies undertaken in the past on factors affecting life expectancy considering demographic variables, income composition and mortality rates. It was found that affect of immunization and human development index was not taken into account in the past. Also, some of the past research was done considering multiple linear regression based on data set of one year for all the countries. Hence, this gives motivation to resolve both the factors stated previously by formulating a regression model based on mixed effects model and multiple linear regression while considering data from a period of 2000 to 2015 for all the countries. Important immunization like Hepatitis B, Polio and Diphtheria will also be considered. In a nutshell, this study will focus on immunization factors, mortality factors, economic factors, social factors and other health related factors as well. Since the observations this dataset are based on different countries, it will be easier for a country to determine the predicting factor which is contributing to lower value of life expectancy. This will help in suggesting a country which area should be given importance in order to efficiently improve the life expectancy of its population.

## Content
The project relies on accuracy of data. The Global Health Observatory (GHO) data repository under World Health Organization (WHO) keeps track of the health status as well as many other related factors for all countries The data-sets are made available to public for the purpose of health data analysis. The data-set related to life expectancy, health factors for 193 countries has been collected from the same WHO data repository website and its corresponding economic data was collected from United Nation website. Among all categories of health-related factors only those critical factors were chosen which are more representative. It has been observed that in the past 15 years , there has been a huge development in health sector resulting in improvement of human mortality rates especially in the developing nations in comparison to the past 30 years. Therefore, in this project we have considered data from year 2000-2015 for 193 countries for further analysis. The individual data files have been merged together into a single data-set. On initial visual inspection of the data showed some missing values. As the data-sets were from WHO, we found no evident errors. Missing data was handled in R software by using Missmap command. The result indicated that most of the missing data was for population, Hepatitis B and GDP. The missing data were from less known countries like Vanuatu, Tonga, Togo, Cabo Verde etc. Finding all data for these countries was difficult and hence, it was decided that we exclude these countries from the final model data-set. The final merged file(final dataset) consists of 22 Columns and 2938 rows which meant 20 predicting variables. All predicting variables was then divided into several broad categories:​Immunization related factors, Mortality factors, Economical factors and Social factors.

## Acknowledgements
The data was collected from WHO and United Nations website with the help of Deeksha Russell and Duan Wang.

## About
This is the mini project for NTU-SC1015 (Introduction to Data Science and Artificial Intelligence).
Singapore ranks as 6th blue zone having one of the highest longevigity age, hence it is crucial for us to explore into factor that affect the life expectancy in the world. In this project, our group's main focus is to analyse the relationship between life expectancy and top 3 variables/factors. The approaches includes/involves both predictive modelling and clustering methods. Predictive modelling helps us predict life expectancy based on the top 3 variables we have chosen based on the correlation plot. In addition to that, clustering helps us identify groups within the expectancy data based on the various factors, helping us further understand about patterns regarding life expectancy. By combining these methods, we aim to get better understanding about the factors that affect life expectancy.

## Problem definition
1. Which of the variables is the best in terms of predicting life expectancy?
2. Which model would be the best in helping us to predict the life expectancy?

## Dataset used
The dataset used for this project is retrieved from [here](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data)

For the cleaned dataset, please download it from [here](https://github.com/zhihaolaw/SC1015/blob/main/cleaned_life_expectancy_data.csv)

## Presentation
Link to the presentation video from [here]()

## Brief process walkthrough

**[Data Preparation & Cleaning]** - Zhi Hao
   1. rename columns of dataframe
   2. data extraction - Justin
   3. KNNImputer for replace null value value
   4. replace oulier with mean value

**[Exploratory Data Analysis]** - Zhi Hao
   1. bi-variante analysis and visualization
   2. uni-variante analysis and visualization
   
**[Machine Learning Model]**
   1. Decision Trees
   2. Linear Regression
   3. Support Vector Regression
   4. Random Forest Regression
   5. K-Means Clustering 


## Conclusion


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


