# Introduction to Data Science course 2023 - advisory report
In the report, we focused on the implementation of three 
models: Decision Tree Classifier, Support Vector Machine Classifier and Logistic 
Regression in the hiring process for a sports recruitment company. The name of 
the company is A and the sports involving the company are swimming, football and 
golf
# Data understanding
Firstly, we read the data into pandas dataframe and displayed it. Our data is from 
the company A and includes Golf, Football and Swimming as sports. We started to 
explore the data. We applied .head(), shape(), describe(), value_counts(). The 
data was read correctly. We checked for the missing values, which were not 
present.
# Data visualisation
- Age distribution by Gender (violin plot)
- Exam score distribution by nationality (violin plot)
- Frequency of individuals knowing additional language (histogram)
- Age distribution of individuals (histogram)
# Probability of being hired for various subgroups
- International experience and age vs. Hiring Probability 
- University grade and gender vs. Hiring Probability
- Age and Entrepreneur Experience vs. Hiring Probability
- University Grade and Debate Club vs. Hiring Probability
# Data preparation
In order to prepare our data, we first check for outliers, missing values and 
duplicates. We did not find any of these and did not remove an data points from 
the data frame. We then split the data into train and test sets with a 80 to 20 
percent ratio.
Then, we decided to One-Hot Encode the Categorical Variables and use a 
Standard Scaler for the Numerical values. We used a Standard Scaler so that the 
data is normally distributed and easier for the model to interpret
# Models Comparison
In this classification task the team focused on SVM
and Decision Tree, because those methods are well
suited for both classification and regression tasks.
Moreover, logistic regression focuses on binary
classification tasks, which meets the objective of the
task.

# Final models exploration
- Are the models biased?
- Decision Tree Model Performance and Hiring Probabilities
- Logistic Regression Model Performance and Hiring Probabilities
- Support Vector Machines Performance and Hiring Probabilities
# Conclusion
After trying out three distinct classification models for predicting the hiring 
decision, we have observed that the best model is the Support Vector Machines 
model, as it has the best overall performance on the test data. It is also the fairest 
of the models, however still not a truly fair method, for the following reason: there 
is still bias towards sensitive features such as gender, nationality and age, in a 
measure that is beyond our acceptable threshold. Therefore, we would recommend to use the model, but with caution and we would advise to hire someone who would make sure that the bias is within acceptable threshold.
