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
print("Array after inserting new column:\n", arr_modified)
Add code here
```
## Output
<img width="1030" height="596" alt="exp1" src="https://github.com/user-attachments/assets/03d92933-8085-422c-8d31-5682c81c9635" />

## Result
The program successfully deletes the second column from 2D array using numpy
