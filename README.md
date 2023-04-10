# Ex03-Univariate-Analysis

AIM:
To read the given data and perform the univariate analysis with different types of plots.

EXPLANATION:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

ALGORITHM:
STEP1:
Read the given data

STEP2:
Get the information about theb data.

STEP3:
Remove the null values from the data.

STEP4:
Mention the datatypes from the data.

STEP5:
Count the values from the data.

STEP6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

PROGRAM:
DEVELOPED BY: JAYAKRISHNAN L B L REG NO: 212222230052

import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("SuperStore.csv")
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x="Postal Code", data=df)
sns.countplot(x="Postal Code", data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x="Postal Code", data=df)
OUTPUT:
Dataset:


Head:


Info:

Describe:


Isnull:

Datatypes:

Value count:


Boxplot:


Countplot:


Distribution plot:

Histogram plot:


RESULT:
Thus we have read the given data and performed the univariate analysis with different types of plots.
