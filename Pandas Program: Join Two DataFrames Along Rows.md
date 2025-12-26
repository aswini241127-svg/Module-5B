# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd
df1 = pd.DataFrame({
    'A': [1, 2, 3],
    'B': ['a', 'b', 'c']
})
df2 = pd.DataFrame({
    'A': [4, 5, 6],
    'B': ['d', 'e', 'f']
})
df_new = pd.concat([df1, df2], axis=0, ignore_index=True)
print("New DataFrame after row-wise concatenation:")
print(df_new)
```

## Output
<img width="1266" height="645" alt="exp1" src="https://github.com/user-attachments/assets/4615884e-7dc5-41ba-a300-ee0b7b4966e4" />

## Result
The program successfully join two DataFrames along rows (row-wise concatenation) and assign all data to a new DataFrame.
