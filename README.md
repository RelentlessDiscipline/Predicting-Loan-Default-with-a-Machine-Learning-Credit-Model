This project I first used Pandas for Data Exploration and Data Cleaning. Then I tried to predict which customer is going to default on their loans using a Machine Learning model called Decision Tree.

The dataset is sourced from kaggel.com (https://www.kaggle.com/skihikingkevin/online-p2p-lending). It combines historical loans from both Prosper and Lending Club from 2013 to 2018.

![image](https://github.com/user-attachments/assets/9d3d73f0-7c1e-4bad-893c-0e6cb67ee53d)


**Data Exploration**

Data exploration aims to understand what data exists in a dataset, its characteristics, and the relationship between elements of the data.
Data exploration has the following stages:
1. Variable identification
2. Data structuring
3. Univariate analysis
4. Bivariate analysis
5. Missing value analysis
6. Outlier analysis

**Data Preparation** 

In this stage we make changes to the dataset so that it can feed nicely into the Machine Learning Models. Data Cleaning usually involves at least one of the below processes:
- Dealing with inconsistent recording
- Removing unwanted observations
- Removing duplicates
- Investigating outliers
- Dealing with missing items

**Splitting Data into Training Data and Test Data**

'loan_status_description' will be our 'target' for the Machine Learning model to learn from and predict. Before we feed the clean dataset into the model, we will split the dataset into training data and testing data. The ML model will train on the training dataset and we will observe the model accuracy by feeding test data into the model for predicted targets.

In general, we will split the dataset 70/30. 70% of data will be used as training data and 30% for testing.

Because most bankruptcy/bad debt data is imbalanced, i.e only a small percentage of data is bankrupt. We need to make sure that both the training and testing dataset has the same proportion of bankruptcy.
![image](https://github.com/user-attachments/assets/b79486ef-5f55-4c8b-8ded-e4328c5029fd)

In the second part I examined missing data and outliers and took appropriete measures to address them. 

Then I explored multicollinearity by calculating VIF (Variance Inflation Factor) for each predictor variable.

Lastly I developed 3 sets of algorithms involving different data treatment, and experimented with Logistic Regression since linear and multilinear regression are less suitable for binary outcomes because they predict continuous values, which may not make sense for the binary classifications.

You can find the model evaluation at the bottom of the project.

Thank you for reading!
