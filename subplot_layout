# Create a series of plots to analyze a given dataset.

# INPUT
# DatasetPlotsSubplots.py
import pandas as pd
import matplotlib.pyplot as plt

# Sample dataset
data = {
    'Name': ['Alice','Bob','Charlie','David','Eva'],
    'Age': [25, 30, 35, 40, 28],
    'Salary': [50000, 60000, 75000, 80000, 52000],
    'Department': ['HR','IT','IT','Finance','HR']
}

df = pd.DataFrame(data)

# Create figure with 2 rows and 3 columns of subplots
fig, axes = plt.subplots(2, 3, figsize=(18, 10))
fig.suptitle("Dataset Analysis Plots", fontsize=16)

# 1 Line plot (Salary vs Age)
axes[0, 0].plot(df['Age'], df['Salary'], marker='o', linestyle='-', color='b')
axes[0, 0].set_title('Line Plot: Salary vs Age')
axes[0, 0].set_xlabel('Age')
axes[0, 0].set_ylabel('Salary')
axes[0, 0].grid(True)

# 2 Bar plot (Salary by Name)
axes[0, 1].bar(df['Name'], df['Salary'], color='green')
axes[0, 1].set_title('Bar Plot: Salary by Name')
axes[0, 1].set_xlabel('Name')
axes[0, 1].set_ylabel('Salary')

# 3 Histogram (Age distribution)
axes[0, 2].hist(df['Age'], bins=5, color='orange', edgecolor='black')
axes[0, 2].set_title('Histogram: Age Distribution')
axes[0, 2].set_xlabel('Age')
axes[0, 2].set_ylabel('Frequency')

# 4 Scatter plot (Age vs Salary)
axes[1, 0].scatter(df['Age'], df['Salary'], color='red')
axes[1, 0].set_title('Scatter Plot: Age vs Salary')
axes[1, 0].set_xlabel('Age')
axes[1, 0].set_ylabel('Salary')

# 5 Pie chart (Department distribution)
dept_counts = df['Department'].value_counts()
axes[1, 1].pie(dept_counts, labels=dept_counts.index, autopct='%1.1f%%', startangle=140)
axes[1, 1].set_title('Pie Chart: Department Distribution')

# Hide the last subplot (empty)
axes[1, 2].axis('off')

plt.tight_layout(rect=[0, 0, 1, 0.96])
plt.show()
