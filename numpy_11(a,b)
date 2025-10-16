# Write a NumPy program using NumPy methods – max, min, argmax, argmin, argmax, repr, count, bincount, unique.
# a. To extract all numbers from a given array which are less and greater than a specified number.
# b. To find the indices of the maximum and minimum numbers along the given axis of an array.

# INPUT

import numpy as np
x = np.array(list(map(int,input("Enter numbers for array (space-separated): ").split())))
print("Array :",x)

# a. Extract numbers less than and greater than a specified number
num = int(input("Enter a number to compare: "))
less_than = x[x<num]
greater_than = x[x>num]
print(f"Number less than {num}:",less_than)
print(f"Numbers greater than {num}:", greater_than)

# b. Find indices of max and min values
print("\nMaximum value:", np.max(x))
print("Index of maximum value:", np.argmax(x))
print("Minimum value:", np.min(x))
print("Index of minimum value:", np.argmin(x))

# Additional NumPy methods
print("\nUsing repr():", repr(x))
print("Unique values:", np.unique(x))
print("Count of each value (using bincount):", np.bincount(x))

# Example for 2D array to show axis-based argmax/argmin
arr2 = np.array([[5, 12, 7], [3, 8, 10]])
print("\n2D Array:\n", arr2)
print("Index of max in each row:", np.argmax(arr2, axis=1))
print("Index of min in each column:", np.argmin(arr2, axis=0))

# OUTPUT
"""
Enter numbers for array (space-separated): 1 2 3 4 5 6 7 8 9 10
Array : [ 1  2  3  4  5  6  7  8  9 10]
Enter a number to compare: 5
Number less than 5: [1 2 3 4]
Numbers greater than 5: [ 6  7  8  9 10]

Maximum value: 10
Index of maximum value: 9
Minimum value: 1
Index of minimum value: 0

Using repr(): array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10])
Unique values: [ 1  2  3  4  5  6  7  8  9 10]
Count of each value (using bincount): [0 1 1 1 1 1 1 1 1 1 1]

2D Array:
 [[ 5 12  7]
 [ 3  8 10]]
Index of max in each row: [1 2]
Index of min in each column: [1 1 0]

"""
