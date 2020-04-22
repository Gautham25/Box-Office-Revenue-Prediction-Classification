# Box-Office-Revenue-Prediction-Classification

In this project, I will be using of dataset that contains movie metadata from Kaggle website. As part of the project, the data pre-processing will be performed in order to clean the data, replace missing values. Feature selection will be performed in order to keep only the relevant features that will be useful for the final analysis. Text analysis will be performed on the Synopsis feature in the dataset in order to extract keywords that will be used as part of the analysis in subsequent steps. The main goal of the project is given a set of features such as genre, keywords, budget, etc. about a movie, the created model will be able to predict the revenue that can be generated based on the information that the model has learned using data from similar movies.

The dataset used in this project was taken from Kaggle which is an online community for data scientists and machine learning practitioners. The dataset contains metadata for 45,000 movies listed in the MovieLens Dataset.

Link: https://www.kaggle.com/rounakbanik/the-movies-dataset


Keeping the final goal of this project, i.e. to predict the revenue based on a set of features, we performed data preprocessing. This involved the following steps:

•	Remove records which had no revenue or blank

•	Fill in the missing values in the budget field with the median of the column values

•	Remove records whose overview was not in English as NLP was one of the major parts of this project

•	Create a one-hot-encoding for the genres as many records had multiple genres

•	Create a feature called “vote_total” which was the product of the columns “vote_average” and “vote_count”. 


Categorization of revenue for classification:

CLASS	    |    Revenue Value

low-profit |   value <= 9631905.25

profit	   |  9631905.25< value <=99347600.25

high-profit  |  value > 99347600.25


The following regression techniques were used to predict the revenue box office in US dollars:

•	Linear Regression

•	Random Forest Regressor

•	Neural Networks


The following classfication techniques were used to predict the category of the predicted revenue:

•	Logistic Regression

•	Random Forest Classifier

•	Support Vector Classifier(SVC) with NLP

•	Neural Networks
