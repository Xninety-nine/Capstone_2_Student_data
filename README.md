# Capstone_2_Student_data
Capstone 2 Project (Student Performance)

Student academic performances in math and reading in the USA fall below that of students from other developed countries, even though the use spends the second most amount of money per student. My goal is to develop ML models that help make schools more efficient with time and money by predicting grades and academic level of students. Administrators usually build schedules for students in the summer and being able to identify students at risk will help them determine how much intervention will be needed for the academic year. Additionally being able to identify students who are academically excelling will help inform teachers on rigor of lessons to promote academic growth. 



In clean_process_student data features are created to calculate average grades earned by students for the year. Absence feature is created to calculate absence as a percent.EDA is performed to get a sense of the data set. Additionally I create categorical features to label students based on the percentlie of their average grade 'Very low'-'very high'. Categorical and object features are also transformed using one-hot encoding to prepare data for modeling.



In modeling_ Linear Regression model, Random Forest Regressor, Gradient Boost Regressor  models are explored to predict grades. Additionallly a logistic regression model is used to try and predict category that student will fall into i.e. ('very low', 'low', 'average', 'high', 'very high')


In predict_studetn_category I perform hyperparameter tunning on both regression and classification models to find optimal performance metrics. I 
