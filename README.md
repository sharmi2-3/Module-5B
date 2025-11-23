# 5A.NumPy Program: Column-wise Sorting of a 2D Array

##  Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

##  Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

##  Program
```
import numpy as np
array = np.array(eval(input()))
print('Given array','\n',array)
print()
print(np.sort(array,axis=0))
```

## Output
<img width="445" height="140" alt="image" src="https://github.com/user-attachments/assets/4525b175-ea07-4cdf-acb1-679f30fa8f72" />


## Result
Thus,the python program has been executed successfully

## 5B. NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

##  Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

##  Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

##  Program
```
import numpy as np
x=np.array(eval(input()))
y=np.array(eval(input()))
print(np.where(x>y))
print(np.where(x==y))
```
## Output
<img width="255" height="147" alt="image" src="https://github.com/user-attachments/assets/08dbd23a-e1e4-408e-9540-a8f2a7777125" />
<img width="196" height="147" alt="image" src="https://github.com/user-attachments/assets/0362968a-3814-4782-926c-ba370091b345" />
<img width="224" height="147" alt="image" src="https://github.com/user-attachments/assets/c2c4648f-b6a3-4b5d-953b-543e262a1c2b" />


## Result
Thus,the python program has been executed successfully

# 5C.NumPy Program: Replace the Second Column in a 2D Array

##  Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

##  Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

##  Program
```
import numpy as np
original=np.array(eval(input()))
newone=np.array(eval(input()))
print("Printing Original array")
print(original)
modified=np.delete(original,1,axis=1)
print("Array after deleting column 2 on axis 1")
print(modified)
result=np.insert(modified,1,newone,axis=1)
print("Array after inserting column 2 on axis 1")
print(result)
```

## Output
<img width="593" height="190" alt="image" src="https://github.com/user-attachments/assets/ae5162bd-8fc8-4e08-84a1-9959f2ed6cee" />

## Result
Thus,the python program has been executed successfully

# 5D.Pandas Program: Create and Display a DataFrame with Custom Index Labels

##  Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

##  Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.



## Program
```
import pandas as pd


data = eval(input())
Col=eval(input())


qrtsales = pd.DataFrame(data,columns=Col)


print (qrtsales)

qs=qrtsales.groupby('itemcat')
print('Result after Filtering Dataframe') 
print(qs['expenditure'].sum())
```
## Output

<img width="441" height="318" alt="image" src="https://github.com/user-attachments/assets/42554f16-8e08-41f5-be79-3558a27f076b" />

## Result
Thus,the python program has been executed successfully

# 5E.Pandas Program: Join Two DataFrames Along Rows

##  AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

##  ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

##  Program
```
import pandas as pd
student_data1 = pd.DataFrame(eval(input()))
student_data2 = pd.DataFrame(eval(input()))
print("Original DataFrames:")
#Add your code here
print(student_data1)
print("-------------------------------------")
print(student_data2)
print()
print("Join the said two dataframes along rows:")
result_data=pd.concat([student_data1,student_data2],ignore_index=False)
print(result_data)
```
## Output
<img width="439" height="278" alt="image" src="https://github.com/user-attachments/assets/7a1f5db0-8c7f-4df0-90d7-1dfc7f1c7b8d" />
<img width="446" height="279" alt="image" src="https://github.com/user-attachments/assets/0ef2a89c-a300-420e-8b89-b35d02aaea1c" />



## Result
Thus,the python program has been executed successfully
