# Example of Logistic Regression in Python
**Steps to Apply Logistic Regression in Python**

1. **Step 1: Gather your data**
    - To start with a simple example, let’s say that your goal is to build a logistic regression model in Python in order to 
       determine whether candidates would get admitted to a prestigious university.
    - Here, there are two possible outcomes: Admitted (represented by the value of ‘1’) vs. Rejected (represented by the 
       value of ‘0’)

**You can then build a logistic regression in Python, where:**
- The dependent variable represents whether a person gets admitted; and
- The 3 independent variables are the GMAT score, GPA and Years of work experience

![screenshot_20210917_190611](https://user-images.githubusercontent.com/47748059/133827113-cf980c89-b1f2-4d59-b214-3a9abc64bc83.png)

**Note that the above dataset contains 40 observations. In practice, you’ll need a larger sample size to get more accurate results.**

2. **Step 2: Import the needed Python packages**

   Before you start, make sure that the following packages are installed in Python:
- `pandas `– used to create the DataFrame to capture the dataset in Python (reading and writing data )
- `sklearn `– used to build the logistic regression model in Python (efficient tools for predictive data analysis)
- `seaborn `– used to create the Confusion Matrix (Python data visualization library)
- `matplotlib `– used to display charts

You’ll then need to import all the packages as follows:

```
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn import metrics
import seaborn as sn
import matplotlib.pyplot as plt
```

3. **Step 3: Build a dataframe**
For this step, you’ll need to capture the dataset (from step 1) in Python. You can accomplish this task using `pandas Dataframe:`
```
import pandas as pd
candidates = {'gmat': [780,750,690,710,680,730,690,720,740,690,610,690,710,680,770,610,580,650,540,590,620,600,550,550,570,670,660,580,650,660,640,620,660,660,680,650,670,580,590,690],
              'gpa': [4,3.9,3.3,3.7,3.9,3.7,2.3,3.3,3.3,1.7,2.7,3.7,3.7,3.3,3.3,3,2.7,3.7,2.7,2.3,3.3,2,2.3,2.7,3,3.3,3.7,2.3,3.7,3.3,3,2.7,4,3.3,3.3,2.3,2.7,3.3,1.7,3.7],
              'work_experience': [3,4,3,5,4,6,1,4,5,1,3,5,6,4,3,1,4,6,2,3,2,1,4,1,2,6,4,2,6,5,1,2,4,6,5,1,2,1,4,5],
              'admitted': [1,1,0,1,0,1,0,1,1,0,0,1,1,0,1,0,0,1,0,0,1,0,0,0,0,1,1,0,1,1,0,0,1,1,1,0,0,0,0,1]
              }

df = pd.DataFrame(candidates,columns= ['gmat', 'gpa','work_experience','admitted'])
print (df)
```
Alternatively, you could import the data into Python from an external file.

4. **Step 4: Create the logistic regression in Python**
set the independent variables\
```
X = df[['gmat', 'gpa','work_experience']]
y = df['admitted']
```
Then, apply train_test_split. For example, you can set the test size to 0.25, and therefore the model testing will be based on 25% of the dataset, while the model training will be based on 75% of the dataset:
`X_train,X_test,y_train,y_test = train_test_split(X,y,test_size=0.25,random_state=0)
`
Apply the logistic regression as follows:

```
logistic_regression= LogisticRegression()
logistic_regression.fit(X_train,y_train)
y_pred=logistic_regression.predict(X_test)
```
Then, use the code below to get the Confusion Matrix:

```
confusion_matrix = pd.crosstab(y_test, y_pred, rownames=['Actual'], colnames=['Predicted'])
sn.heatmap(confusion_matrix, annot=True)
```
For the final part, print the Accuracy and plot the Confusion Matrix:

```
print('Accuracy: ',metrics.accuracy_score(y_test, y_pred))
plt.show()
```
**Run the code in Python, and you’ll get the following Confusion Matrix with an Accuracy of 0.8 (note that depending on your sklearn version, you may get a different accuracy results. In my case, the sklearn version is 0.22.2):**

![screenshot_20210917_193142](https://user-images.githubusercontent.com/47748059/133830105-55d35187-344e-466b-b7af-c95bb922c9ab.png)


As can be observed from the matrix:

- TP = True Positives = 4
- TN = True Negatives = 4
- FP = False Positives = 1
- FN = False Negatives = 1

Accuracy = (TP+TN)/Total = (4+4)/10 = 0.8
The accuracy is therefore 80% for the test set.

