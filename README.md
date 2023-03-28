# Ex03-Univariate-Analysis
# Aim
To read the given data and perform the univariate analysis with different types of plots.
Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
# Algorithm
# Step1
Read the given data.

# Step2
Get the information about the data.

# Step3
Remove the null values from the data.

# Step4
Mention the datatypes from the data.
# Step5
Count the values from the data.

# Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program

``` 
Developed by        : IRENE JECINTHA MERLIN R
Registration Number : 212221040058

import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
# Output
# DATA
## ![image](https://user-images.githubusercontent.com/128350225/228207820-da3e5459-89d0-47ae-a58e-83111b8ce18e.png)
DATA HEAD
## ![image](https://user-images.githubusercontent.com/128350225/228208096-4a9606b2-0aa9-4f9b-982b-66892318b0dd.png)
# DATA INFORMATION
## ![image](https://user-images.githubusercontent.com/128350225/228208224-1112fc86-7cfc-4ef9-9b83-c072c60b4dea.png)
# DATA DESCRIBE
## ![image](https://user-images.githubusercontent.com/128350225/228208894-6d9b4082-00da-4d5c-94fa-3ad244fad23c.png)
# DATA NULL VALUES
## ![image](https://user-images.githubusercontent.com/128350225/228209118-c29aaabe-1cb6-4a08-aa80-c390f7e3fa85.png)
# DATA'S DATATYPES
## ![image](https://user-images.githubusercontent.com/128350225/228209240-72e3b9cc-93d9-4ed4-b91f-4c4e7ed3f7a3.png)
# DATA'S VALUECOUNT
## ![image](https://user-images.githubusercontent.com/128350225/228209353-835a5208-1509-4099-91ed-c4a9fa027890.png)
# BOXPLOT
## ![image](https://user-images.githubusercontent.com/128350225/228209469-6aa18614-19ae-4872-ba71-36371fe88fc9.png)
# COUNTPLOT
## ![image](https://user-images.githubusercontent.com/128350225/228209631-757b6d2d-22d4-4595-928f-4795650b69f8.png)
# DISTRIBUTION PLOT
## ![image](https://user-images.githubusercontent.com/128350225/228209790-69d03248-5b8c-4df4-8fe1-43d738e5c6e6.png)
# HISTOGRAM PLOT
## ![image](https://user-images.githubusercontent.com/128350225/228209910-802d1c28-a0b0-49cc-8706-36ae5b50ce55.png)
# Result
Thus we have read the given data and performed the univariate analysis with different types of plots.

