# Pandas DataSeries:
# a. Write a Pandas program to create and display a one-dimensional array-like object containing an array of data using Pandas module.
# b. Write a Pandas program to convert a Panda module Series to Python list and it's type.

# INPUT

import pandas as pd

# a. User input to create a Series
x = list(map(int,input("Enter numbers for Series (space-separated): ").split()))
y = pd.Series(x)
print("\nPandas Series:")
print(y)

# b. Convert Series to Python list and check type
z = y.tolist()
print("\nConverted to Python list:", z)
print("Type of converted data:", type(z))

# OUTPUT
"""
Enter numbers for Series (space-separated): 12 14 15 16 13 14

Pandas Series:
0    12
1    14
2    15
3    16
4    13
5    14
dtype: int64

Converted to Python list: [12, 14, 15, 16, 13, 14]
Type of converted data: <class 'list'>
"""
