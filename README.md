# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np

# Accept input for 2D array
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter the elements row-wise (space-separated):")
arr = []
for i in range(rows):
    arr.append(list(map(int, input().split())))

# Convert to NumPy array
array = np.array(arr)

# Column-wise sorting
sorted_array = np.sort(array, axis=0)

# Display results
print("\nOriginal Array:")
print(array)

print("\nColumn-wise Sorted Array:")
print(sorted_array)
```

## Output
<img width="692" height="408" alt="exp1" src="https://github.com/user-attachments/assets/90cd1334-e10a-4104-a0a0-86c30403b9d5" />

## Result
The program successfully accepts a 2D array from the user, sorts each column in ascending order, and prints both the original and column-wise sorted arrays using NumPy.
# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
```
import numpy as np
x = np.array([5, 3, 7, 1, 9])
y = np.array([2, 4, 7, 0, 10])
indices = np.where(x >= y)[0]

print("Indices where x >= y:", indices)
```
## Output
<img width="805" height="377" alt="exp1" src="https://github.com/user-attachments/assets/f62e5709-4b7e-4d9e-8e21-ef8649d294a9" />

## Result
The program successfully finds the indices where elements in array x are greater than or equal to their corresponding elements in array y.
# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

```import numpy as np

# Define the original 2D array
arr = np.array([[1, 2, 3],
                [4, 5, 6],
                [7, 8, 9]])

# Delete the second column (index 1)
arr_deleted = np.delete(arr, 1, axis=1)

# Define the new column to insert
new_col = np.array([10, 11, 12])

# Insert the new column at the same position (index 1)
arr_modified = np.insert(arr_deleted, 1, new_col, axis=1)

print("Original array:\n", arr)
print("Array after deleting second column:\n", arr_deleted)
print("Array after inserting new column:\n", arr_modified)``

Add code here
```
## Output
<img width="814" height="365" alt="exp1" src="https://github.com/user-attachments/assets/49a03c5b-ed4f-4a99-84e0-9da7bc78ea6a" />

## Result
The program successfully deletes the second column from 2D array using numpy
