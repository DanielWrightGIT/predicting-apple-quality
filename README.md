# 🍎 Predictive Classification of Apples 🍎

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data](#data)
3. [Methodology](#Methodology)
4. [EDA](#EDA)
5. [Modification of Data](#modification-of-data)
6. [Visualization](#visualization)
7. [Discussion of Results](#Discussion-of-Results)


### Project Overview
The purpose of this project is to create predictive classifiers to determine the quality of apples. These predictions are based on variables related to the quality of apples using features such as ripeness, crunchiness, weight, acidity, etc. The models can be utilized by farmers or produce sellers to determine the financial value of their product or to predict the quality of future anticipated harvests.


### Data
The data was retrieved in the form of a CSV file from Kaggle.com and uploaded by Nidula Elgiriyewithana who states that the set was provided by a nameless American agriculture company. https://www.kaggle.com/datasets/nelgiriyewithana/apple-quality


### Methodology
- Python: EDA, modification, cleaning, and modeling


### EDA
The uploader kindly took the liberty of scaling and cleaning the data. There were some remaining NA values which I cleaned prior to modeling.


### Modification of Data
- Column: A_id | Represents unique identifiers for each fruit. This feature was not required for modeling and was dropped from the dataframe.
- Column: Quality | Initially the quality of the apples was listed as either "good" or "bad". For the sake of convenience these values were re-mapped to numerical binary values. Good apples are transformed to "1" and bad apples are "0"


### Visualization
The data can be visualized utilizing a kernel density estimate (KDE) plot which covers all of the variables in the set.
![Apple KDE](https://github.com/DanielWrightGIT/Apple-quality-prediction/assets/158070869/cfa5411d-f055-454f-84de-92335a698573)



### Discussion of Results
![model accuracy](https://github.com/DanielWrightGIT/Apple-quality-prediction/assets/158070869/41714cc7-629f-4ecc-8d78-8475bc3d0467)

Observing the results the K-Nearest Neighbor(KNN) model is the most accurate at 90.08% while our least accurate model is Naive Bayes at 72.25%. Ideally we would like to see values of >= 85% and 6 out of 10 models were able to meet this success rate. Implementation of the KNN model will lead to accurate predictions in 9 out of 10 evaluations.
