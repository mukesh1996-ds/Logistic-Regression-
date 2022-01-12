# Logistic-Regression-
```
This is the task in Machine Learning.

```
# Data set 

```
The dataset I chose is the affairs dataset that comes with Statsmodels. It was derived from a survey of women in 1974 by Redbookc magazine, in which married women were asked about their participation in extramarital affairs. More information about the study is available in a 1978 paper from the Journal of Political Economy.

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
from sklearn.linear_model
import LogisticRegression from
sklearn.cross_validation
import train_test_split from sklearn
import metrics from
sklearn.cross_validation
import cross_val_score dta =
sm.datasets.fair.load_pandas().data

```
