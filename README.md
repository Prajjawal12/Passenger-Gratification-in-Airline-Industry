# Passenger Gratification in Airline Industry
## Objective
The aim of this project is to assist an airline company in identifying the key factors that influence passenger gratification. Ensuring high levels of passenger happiness is crucial for boosting a company's business, reputation, and overall growth. By analyzing and enhancing the factors most closely related to passenger gratification, the airline can soar to new heights! 🚀

*This project leverages the* ***CRISP-DM methodology*** *to find the best solution to this business challenge. The process is carried out through six phases: Business Understanding, Data Understanding, Data Preparation, Data Modeling, Evaluation, and Deployment.*

## About the Data
The dataset for this project was sourced from Kaggle, based on a survey conducted by airlines to measure passengers' gratification levels across various factors. It contains 25 columns, including details like Age, Gender, Travel Class, Arrival and Departure Delays, and features influencing passenger gratification such as On-board Service, Cleanliness, Seat Comfort, Baggage Handling, and more.

A special column named ***‘satisfaction’*** indicates the overall gratification level of the passengers, categorized into two values: ‘neutral or dissatisfied’ and ‘satisfied’. This ***satisfaction*** feature serves as the label, reflecting the overall passenger experience based on their ratings for other factors. The dataset includes 103,904 records in the training set and 25,976 records in the test set.

## Data Cleaning and Visualization
Data cleaning is essential for achieving accurate results with a machine learning model. This process typically involves identifying and addressing outliers, filling in missing values, removing duplicates, and eliminating values with little or no significance.

In this project, the *‘Arrival Delay in Minutes’* column had 310 missing values, which were imputed using the mean of the available data.

Visualizing the data is equally important, as it provides an overview of the dataset before diving into modeling. Exploratory Data Analysis (EDA) was conducted to better understand the data.

## Feature Selection
Correlation among features was examined using a correlation matrix, and the top ten features were selected using the Chi-Square method. Feature importance was assessed using the Wrapper method and feature permutation importance technique to determine which features most influence passenger gratification.

## Models
To achieve the best possible results, eight models were employed:
- Logistic Regression
- Naive Bayes
- KNN
- Decision Tree
- Neural Network
- Random Forest
- XGBoost
- AdaBoost

## Conclusion
Both Random Forest and AdaBoost delivered impressive results with high ROC_AUC scores (~90%). However, ***Random Forest*** emerged as the winner, taking significantly less time to compute compared to AdaBoost. Thus, Random Forest is crowned as the best model! 🏆

## Explanation of Technical Terms and Models

### **CRISP-DM Methodology**
CRISP-DM stands for Cross-Industry Standard Process for Data Mining. It’s a popular methodology used to tackle data mining and machine learning projects. The process includes six phases:
1. **Business Understanding:** Defining the objectives and requirements from a business perspective.
2. **Data Understanding:** Collecting and exploring the data to get insights.
3. **Data Preparation:** Cleaning and transforming the data for modeling.
4. **Modeling:** Applying different algorithms to build models.
5. **Evaluation:** Assessing the models to ensure they meet business objectives.
6. **Deployment:** Implementing the model in a real-world environment.

### **Exploratory Data Analysis (EDA)**
EDA involves analyzing datasets to summarize their main characteristics, often using visual methods. It helps in understanding the structure of the data, detecting outliers, and discovering patterns.

### **Correlation Matrix**
A correlation matrix is a table showing correlation coefficients between variables. It helps in identifying how closely related different features are, which is useful for feature selection.

### **Chi-Square Method**
The Chi-Square method is a statistical test used to determine the independence of two categorical variables. It’s commonly used in feature selection to choose features that have the highest impact on the target variable.

### **Wrapper Method**
The Wrapper Method is a feature selection technique that evaluates subsets of features by training models and selecting the subset that gives the best performance.

### **Feature Permutation Importance**
This technique measures the importance of a feature by observing the decrease in a model’s performance when the values of that feature are randomly shuffled.

### **ROC_AUC Score**
ROC_AUC (Receiver Operating Characteristic - Area Under the Curve) is a performance measurement for classification problems. It shows how well the model distinguishes between classes, with a score closer to 1 indicating a better model.

### **Machine Learning Models:**
- **Logistic Regression:** A statistical model used for binary classification. It predicts the probability of a binary outcome.
- **Naive Bayes:** A probabilistic classifier based on applying Bayes' theorem with strong independence assumptions between the features.
- **K-Nearest Neighbors (KNN):** A simple algorithm that classifies a data point based on the majority class among its nearest neighbors.
- **Decision Tree:** A model that makes decisions based on the answers to a series of questions, structured like a tree.
- **Neural Network:** A computational model inspired by the human brain, consisting of interconnected layers that process data in a hierarchical manner.
- **Random Forest:** An ensemble learning method that constructs multiple decision trees and merges their outcomes to improve accuracy and control overfitting.
- **XGBoost:** An advanced implementation of gradient boosting that is highly efficient, flexible, and portable, often used in competitive machine learning.
- **AdaBoost:** A boosting algorithm that combines the outputs of multiple weak learners to create a strong classifier, focusing on misclassified instances.

