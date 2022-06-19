# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries.
2. Upload and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
5. Find the accuracy of the model and predict the required values by importing the required module from sklearn.
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Rasam Vishnu
RegisterNumber: 212220040131
import pandas as pd
data = pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["salary"] = le.fit_transform(data["salary"])
data.head()
x = data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y = data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt = DecisionTreeClassifier(criterion = "entropy")
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
## Data Head
![4 1](https://user-images.githubusercontent.com/103240414/174469667-3559d1f2-5784-4f98-9650-fdff613a7fea.png)
## Data Info
![4 2](https://user-images.githubusercontent.com/103240414/174469682-5ac4d2a9-70b5-442e-beeb-5b1a7dc299fb.png)
## Data isnull
![4 3](https://user-images.githubusercontent.com/103240414/174469835-87ebdf4d-9601-4d63-962f-667c0a3cd932.png)

## Data Left
![4 4](https://user-images.githubusercontent.com/103240414/174469741-82d820d2-1df0-4a5c-a473-422ee49ba735.png)
## X Head
![4 5](https://user-images.githubusercontent.com/103240414/174469761-77eea9d3-db62-428a-b2fb-720e19804fe9.png)
## Data fit
![4 6](https://user-images.githubusercontent.com/103240414/174469771-5bde43f2-656e-4bba-bf08-f883d7fc5da4.png)
## Accuracy
![4 7](https://user-images.githubusercontent.com/103240414/174469785-7cfb5ead-5d82-466d-a443-ec2333198826.png)
## Predicted Values
![4 8](https://user-images.githubusercontent.com/103240414/174469800-c7fdd477-fa3a-45ba-b529-ca9675a56abe.png)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
