# Titanic Survival Prediction

A logistic regression model that predicts whether a passenger survived the Titanic.

## Data

Titanic-Dataset.csv from Kaggle has one row per passenger (891 rows).

The model uses 7 features:

- Pclass: ticket class (1, 2 or 3)
- Sex: male = 1, female = 0
- Age
- SibSp: siblings or spouses on board
- Parch: parents or children on board
- Fare: ticket price
- Embarked: port of boarding (S = 0, C = 1, Q = 2)

The target is Survived (1 = survived, 0 = did not survive).

## Steps

1. Load the data and check for missing values
2. Fill missing Age values with the mean age
3. Fill missing Embarked values with the most common port
4. Drop the Cabin column because most of its values are missing
5. Convert Sex and Embarked to numbers
6. Drop PassengerId, Name and Ticket
7. Split the data into 80% training and 20% testing
8. Train a logistic regression model
9. Check accuracy on the training and test data
10. Predict survival for a new passenger

## Result

Accuracy on test data: 78%

## Run

```
pip install -r requirements.txt
jupyter notebook titanic.ipynb
```

## Dataset

https://www.kaggle.com/datasets/yasserh/titanic-dataset
