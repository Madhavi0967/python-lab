# Pandas DataFrames:
# Consider Sample Python dictionary data and list labels:
# import pandas as pd
# import numpy as np

# Sample dictionary data
"""
exam_data = {
    'name': ['Anastasia','Dima','Katherine','James','Emily','Michael','Matthew','Laura','Kevin','Jonas'],
    'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
    'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
    'qualify': ['yes','no','yes','no','no','yes','yes','no','no','yes']
}
labels = ['a','b','c','d','e','f','g','h','i','j']
"""
# a. Write a Pandas program to create and display a DataFrame from a specified dictionary data which has the index labels.
# b. Write a Pandas program to change the name 'James' to 'Suresh' in name column of the DataFrame.
# c. Write a Pandas program to insert a new column in existing DataFrame. iv) Write a Pandas program to get list from DataFrame column headers.

# INPUT

import pandas as pd
import numpy as np

# Sample dictionary data
exam_data = {
    'name': ['Anastasia','Dima','Katherine','James','Emily','Michael','Matthew','Laura','Kevin','Jonas'],
    'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
    'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
    'qualify': ['yes','no','yes','no','no','yes','yes','no','no','yes']
}

labels = ['a','b','c','d','e','f','g','h','i','j']

# a. Create and display DataFrame with index labels
x = pd.DataFrame(exam_data, index = labels)
print("Original DataFrame:\n", x)

# b. Change name 'James' to 'Suresh' in 'name' column
x["name"] = x["name"].replace("James","Suresh")
print("\nDataFrame after changing 'James' to 'Suresh':\n", x)

# c. Insert a new column in existing DataFrame
x['city'] = ['Delhi','Mumbai','Chennai','Kolkata','Bangalore','Hyderabad','Pune','Jaipur','Lucknow','Chandigarh']
print("\nDataFrame after adding new column 'city':\n", x)

# d. Get list of DataFrame column headers
y = x.columns.tolist()
print("\nList of DataFrame column headers:", y)

# OUTPUT
"""
Original DataFrame:
         name  score  attempts qualify
a  Anastasia   12.5         1     yes
b       Dima    9.0         3      no
c  Katherine   16.5         2     yes
d      James    NaN         3      no
e      Emily    9.0         2      no
f    Michael   20.0         3     yes
g    Matthew   14.5         1     yes
h      Laura    NaN         1      no
i      Kevin    8.0         2      no
j      Jonas   19.0         1     yes

DataFrame after changing 'James' to 'Suresh':
         name  score  attempts qualify
a  Anastasia   12.5         1     yes
b       Dima    9.0         3      no
c  Katherine   16.5         2     yes
d     Suresh    NaN         3      no
e      Emily    9.0         2      no
f    Michael   20.0         3     yes
g    Matthew   14.5         1     yes
h      Laura    NaN         1      no
i      Kevin    8.0         2      no
j      Jonas   19.0         1     yes

DataFrame after adding new column 'city':
         name  score  attempts qualify        city
a  Anastasia   12.5         1     yes       Delhi
b       Dima    9.0         3      no      Mumbai
c  Katherine   16.5         2     yes     Chennai
d     Suresh    NaN         3      no     Kolkata
e      Emily    9.0         2      no   Bangalore
f    Michael   20.0         3     yes   Hyderabad
g    Matthew   14.5         1     yes        Pune
h      Laura    NaN         1      no      Jaipur
i      Kevin    8.0         2      no     Lucknow
j      Jonas   19.0         1     yes  Chandigarh

List of DataFrame column headers: ['name', 'score', 'attempts', 'qualify', 'city']
"""
