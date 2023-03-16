# DISTANCE-BETWEEN-TWO-POINTS

## AIM:
To write a python program to find the distance two 2 points
## ALGORITHM:
### Step 1: 
Import NumpPy
### Step 2: 
Import Math
### Step 3: 
Get the input for the 2 points
### Step 4: 
Substitute the values in the distance formula  
![image](./formula.JPG)
### Step 5:
Print distance 
### PROGRAM:

```python
import pandas as pd

df = pd.read_csv('credit_data_1.csv')
print(df)
print(df.info())
print(df.isnull())
df['card'] = df["card"].fillna(df['card'].mode()[0])
df['owner'] = df["owner"].fillna(df['owner'].mode()[0])
df['selfemp'] = df["selfemp"].fillna(df['selfemp'].mode()[0])
df.dropna()
df.dropna(axis=0)
df['reports'] = df['reports'].fillna(value=df['reports'].mean())
df['age'] = df['age'].fillna(value=df['age'].mean())
df['income'] = df['income'].fillna(value=df['income'].mean())
df['share'] = df['share'].fillna(value=df['share'].mean())
df['reports'] = df['reports'].fillna(value=df['reports'].mean())
df['expenditure'] = df['expenditure'].fillna(df['expenditure'].median())
df['months'] = df['months'].fillna(df['months'].median())
df['majorcards'] = df['majorcards'].fillna(method='ffill')
df['active'] = df['active'].fillna(method='bfill')
print(df.isnull().sum())

```


### OUTPUT:

recent:///a4b261ac163141a41c27652164135bcb
recent:///95ae53b3e3721999791de61764135bd3

### RESULT:

Thus the distance between two points is found.
