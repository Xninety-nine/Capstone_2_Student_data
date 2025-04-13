## Capstone_2_Student_data
## [Linkedin](https://www.linkedin.com/in/francisco-torres-6a8b65187/)

# Predicting Student Academic Performance

![alt text](image.png)



The United States ranks second in the world for per-student spending, yet academic performance in math and reading often lags behind that of students in other developed countries. This project aims to develop machine learning models that help schools use time and resources more efficiently by predicting students' academic levels and likelihood of class failures.

Accurate predictions can enable administrators to identify at-risk students and allocate intervention resources effectively during schedule planning. Early identification of students likely to struggle can drive timely support, while insights into academically excelling students can inform teachers on lesson rigor to foster continued growth.




1) The data was obtained from [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/320/student+performance)

This data set tracks Portugese student's academic performance through out one school year. The students are ages 15-22. Additional features from this data include: studytime, family relationship, school and family support, amount of free time, absences, health, alochol use and several other features. 



2) In [Loading_cleaning](Loading_Cleaning.ipynb) notebook the dataset is loaded and preprocessed. New features are created, including the calculation of students' average grades for the year and an absence percentage feature. A quick exploratory data analysis (EDA) provides initial insights into the dataset. Additionally, categorical labels ('low', 'average', 'high') are assigned to students based on their average grade percentiles. Categorical and object-type features are then transformed using one-hot encoding to prepare the data for modeling.



3) In [Exploratory_Data_Analysis](Exploratory_Data_Analysis.ipynb) I conduct an in-depth analysis of the data, exploring and visualizing distributions for key features like age, absences, and annual grades. Additionally, I examine the distribution of grades and interactions between variables, such as family support and study time, as well as the relationship between average grade and time spent studying.


<img width="724" alt="image" src="https://github.com/user-attachments/assets/dcbc1268-7457-47e9-8852-735fe01d7cc5" />




4) In [Preprocessing](Preprocessing.ipynb) notebook data transformations are applied to prepare it for machine learning algorithms. Categorical and object-type variables are converted to numeric values using one-hot encoding, and ordinal features are mapped to preserve their inherent order. Additionally, features are scaled and normalized using StandardScaler. Finally, the data is split into training and testing sets, setting the stage for model training and evaluation.




5) In [Machine Learning](Machine_Learning.ipynb) notebook, I develop regression models to predict students' grades and classification models to predict the likelihood of class failures for the academic year. After evaluating baseline models, I perform hyperparameter tuning to improve performance. Finally, I visualize feature importance and classification metrics, including a confusion matrix, to interpret model results effectively.

6) Conclusion:
- Grade Prediction: The RandomForestRegressor with hyperparameter tuning proved to be the best model for predicting students' average grades for the year. With an R-squared score of 0.856, it shows strong predictive capability (where 1.0 is a perfect fit). The model's performance improved significantly after including semester 1 grades in the training data. This model could assist administration and teachers after the first quarter by providing insights into students' likely average grades by year-end.

- Class Failure Prediction: For identifying students at risk of failing a class, the RandomForestClassifier with hyperparameter tuning was the most effective model, achieving a test accuracy of 0.82. It correctly identified students who would pass 88% of the time and accurately predicted those who would fail 60% of the time.
   

7) Next steps: 

- Addressing Class Imbalance: Implement resampling techniques to handle the imbalanced dataset. This could include oversampling methods (e.g., SMOTE) to increase the number of minority class samples or undersampling to reduce the size of the majority class.
- Further Parameter Tuning: Continue exploring hyperparameters to optimize model performance further.
- Feature Engineering: Identify and create additional features to improve the model’s ability to classify students at risk of failing, enhancing the precision of future predictions.
- Create an XGBoost model with hyperparameter tuning and evaluate metrics. 
