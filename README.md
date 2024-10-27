# Capstone_2_Student_data
Capstone 2 Project (Student Performance)

![alt text](image.png)



The United States ranks second in the world for per-student spending, yet academic performance in math and reading often lags behind that of students in other developed countries. This project aims to develop machine learning models that help schools use time and resources more efficiently by predicting students' academic levels and likelihood of class failures.

Accurate predictions can enable administrators to identify at-risk students and allocate intervention resources effectively during schedule planning. Early identification of students likely to struggle can drive timely support, while insights into academically excelling students can inform teachers on lesson rigor to foster continued growth.




1) The data was obtained from [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/320/student+performance)

This data set tracks Portugese student's academic performance through out one school year. The students are ages 15-22. Additional features from this data include: studytime, family relationship, school and family support, amount of free time, absences, health, alochol use and several other features. 



2) In [Loading_cleaning](Loading_Cleaning.ipynb) notebook the dataset is loaded and preprocessed. New features are created, including the calculation of students' average grades for the year and an absence percentage feature. A quick exploratory data analysis (EDA) provides initial insights into the dataset. Additionally, categorical labels ('low', 'average', 'high') are assigned to students based on their average grade percentiles. Categorical and object-type features are then transformed using one-hot encoding to prepare the data for modeling.



3) In [Exploratory_Data_Analysis](Exploratory_Data_Analysis.ipynb) I conduct an in-depth analysis of the data, exploring and visualizing distributions for key features like age, absences, and annual grades. Additionally, I examine the distribution of grades and interactions between variables, such as family support and study time, as well as the relationship between average grade and time spent studying.


4) In [Preprocessing](Preprocessing.ipynb) notebook data transformations are applied to prepare it for machine learning algorithms. Categorical and object-type variables are converted to numeric values using one-hot encoding, and ordinal features are mapped to preserve their inherent order. Additionally, features are scaled and normalized using StandardScaler. Finally, the data is split into training and testing sets, setting the stage for model training and evaluation.




6) In [Machine Learning](MachineLearning.ipynb) notebook, I develop regression models to predict students' grades and classification models to predict the likelihood of class failures for the academic year. After evaluating baseline models, I perform hyperparameter tuning to improve performance. Finally, I visualize feature importance and classification metrics, including a confusion matrix, to interpret model results effectively. 
