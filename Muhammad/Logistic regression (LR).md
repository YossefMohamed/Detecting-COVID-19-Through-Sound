# _What is Regression Analysis?_
**_Regression analysis is a form of predictive modelling technique which investigates the relationship between a dependent (target) and independent variable (s) (predictor). This technique is used for forecasting, time series modelling and finding the causal effect relationship between the variables. For example, relationship between rash driving and number of road accidents by a driver is best studied through regression._**

![Regression_Line](https://user-images.githubusercontent.com/47748059/132488729-df4f5281-81af-48fa-aca9-cd773c171d90.png)

**_Regression analysis is an important tool for modelling and analyzing data. Here, we fit a curve / line to the data points, in such a manner that the differences between the distances of data points from the curve or line is minimized.  I’ll explain this in more details in coming sections._**

# _Why do we use Regression Analysis?_
_As mentioned above, regression analysis estimates the relationship between two or more variables. Let’s understand this with an easy example:_

_Let’s say, you want to estimate growth in sales of a company based on current economic conditions. You have the recent company data which indicates that the growth in sales is around two and a half times the growth in the economy. Using this insight, we can predict future sales of the company based on current & past information._

**_There are multiple benefits of using regression analysis. They are as follows:_**

- _It indicates the significant relationships between dependent variable and independent variable._
- _It indicates the strength of impact of multiple independent variables on a dependent variable._

_Regression analysis also allows us to compare the effects of variables measured on different scales, such as the effect of price changes and the number of promotional activities. These benefits help market researchers / data analysts / data scientists to eliminate and evaluate the best set of variables to be used for building predictive models_

# _A Type Of Regression Is  **Logistic Regression**_
**_Logistic regression is used to find the probability of event=Success and event=Failure. We should use logistic regression when the dependent variable is binary (0/ 1, True/ False, Yes/ No) in nature._**

# What is Logistic regression (LR) ?
- Logistic regression is a popular technique used in machine learning to solve binary classification problems.
- Logistic regression is popular because it provides a simple and powerful method to solve a wide range of problems.
- Logistic regression can be used to predict the probability that a dependent variable belongs to a class, e.g. healthy or sick, given a set of covariates, e.g. some genomic data.

# What is the model training phases ?
 - It starts with a training phase during which one computes a model for prediction based on previously gathered values for predictor variables (called covariates) and corresponding outcomes.
- The training phase is followed by a testing phase that assesses the accuracy of the model. 
- To this end, the dataset is split into data for training and data for validation. This validation is done by evaluating the model in the given covariates and comparing the output with the known outcome.

# How LR be considered to be valuable ?
When the classification of the model equals the outcome for most of the test data, the model is considered to be valuable and it can be used to predict the probability of an outcome by simply evaluating the model for new measurements of the covariates.
# Best Apps for LR Classifier?

- In medicine, logistic regression is used to predict the risk of developing a certain disease based on observed characteristics of the patient.
- In politics, it is used to predict the voting behaviour of a person based on personal data such as age, income, sex, state of residence, previous votes. 
- In finance, logistic regression is used to predict the likelihood of a homeowner defaulting on a mortgage or a credit card transaction being fraudulent.
# DataSet Type Used?
As all machine learning tools, logistic regression needs sufficient training data to construct a useful model. 

# [Reference](https://link.springer.com/article/10.1186/s12920-018-0398-y)


