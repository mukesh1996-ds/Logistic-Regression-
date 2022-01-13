# Logistic-Regression-
```
This is the task in Machine Learning.

```
# Problem statement 

```
The dataset I chose is the affairs dataset that comes with Stats models. It was derived from a survey of women in 1974 by Red book magazine, in which married women were asked about their participation in extramarital affairs.I decided to treat this as a classification problem by creating a new binary variable affair (did the woman have at least one affair?) and trying to predict the classification for each woman.Variables that is present in the dataset for prediction are :-rate_marriage(women’s rating for her marriage) ,age(women’s age),yrs_married(number of years married), children(no. of children she has),religious(on the scale of 1 -5 whether she believe in religion or not),education(level of education), occupation ,occupation of husband, affairs

```
# Description of variables
```
The dataset contains 6366 observations of 9 variables:

rate_marriage: woman&#39;s rating of her marriage (1 = very poor, 5 = very good) age: woman&#39;s age yrs_married: number of years married children: number of children religious: woman&#39;s rating of how religious she is (1 = not religious, 4 =strongly religious) educ: level of education (9 = grade school, 12 = high school, 14 = some college, 16 = college graduate, 17 = some graduate school, 20 = advanced degree) occupation: woman&#39;s occupation (1 = student, 2 = farming/semi- skilled/unskilled, 3 = &quot;white collar&quot;, 4 = teacher/nurse/writer/technician/skilled, 5 = managerial/business, 6 = professional with advanced degree) occupation_husb: husband&#39;s occupation (same coding as above) affairs: time spent in extra-marital affairs

```
# Loading the dataset
```
import numpy as np
import pandas as pd
import statsmodels.api as sm
import matplotlib.pyplot as plt
from patsy import dmatrices
from sklearn.linear_model import LogisticRegression 
from sklearn.model_selection import train_test_split
import metrics from sklearn.cross_validation
import cross_val_score dta = sm.datasets.fair.load_pandas().data

```

# Data preprocessing
```
We want to make it classification problem for that we need to convert target variable (affairs) into binary class where if the value will be 0 then women had no any affair and 1 means women had been involved in several extra marital affairs.

Here we will use pasty.dmatrices, it’s main task is to analyze the independent variable and dependent variable and add some data if it is needed based on target variable.

```
# Local execution 
```
flask 

```
# URL
```
Running on http://127.0.0.1:5000/
```
