
<h2 align="center"> Predict Employee Satisfaction </h2>

### 📌 Project description and methodology

In this project, we will use data science and machine learning techniques to analyze and predict the factors that influence employee satisfaction in a company. The goal is to identify the most significant variables that affect employee well-being and motivation, such as work environment, compensation, growth opportunities, and work-life balance. 
We will use a dataset that includes several employee characteristics, such as age, length of service, performance reviews, feedback, and satisfaction rates.

### 📜 Dataset

The dataset used was extracted from Kaggle and was created by IBM's HR team.

The glossary of the columns is available in the wiki section here on git.

### 📚 Libraries

Python libraries used for this project are:

- sklearn
- pandas

### 📍 Explory Analysis and target variable

For this project, the target variable was set to the "Attrition" column, which corresponds to three situations of the employee in relation to the company. That is, whether he or she is a current employee, whether he or she has resigned or has voluntarily resigned.

The main objective of the model will be to identify which factors led to employees voluntarily resigning.

### ⚙️ Pre-Processing

To create the classification model, the values ​​in the "Attrition" column were converted to a binary classification, where "0" represents the non-occurrence of the event (when there is no voluntary termination, i.e., employees remain employed or have been terminated) and "1" represents the occurrence of the event (when there has been voluntary termination)

  - Numeric Variable Pipeline

  For the numeric variables in the dataset, a pipeline was created to handle missing values, replacing them with the median, and the data was also normalized using StandardScaler.

  - Numeric Variable Pipeline

  As for the numerical categorical variables of the dataset, a pipeline was created to treat the missing values, replacing them with the value ''missing'' and subsequently one-hot encoding was applied, transforming the text data into numerical data for the machine learning process.

###  🗑️ Data Modeling Predictive

n the "Modeling Pipeline" stage, the numerical and categorical variable pipeline stages were concatenated, and the model was trained using the logistic regression algorithm.
the best model performance through GridSearchCV from sklearn.

### 📊 Results

Based on the analysis of the data  logistic regression coefficients, the characteristics that have the greatest relationship with voluntary resignation were: BusinessTravel Travel Frequently, EducationField_Technical Degree and Employee Source_Referral.

![Captura de tela 2025-05-23 181959](https://github.com/user-attachments/assets/43cb3b59-c9fc-4e48-84e2-550dde87b0d8)


