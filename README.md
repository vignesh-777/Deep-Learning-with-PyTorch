# PyTorch Basics Exercises

## AIM:
Write a Python program using PyTorch that performs the following tasks:

### Software Required:
- Python 3.x
- PyTorch
- Jupyter Notebook (for interactive development and execution)

## Algorithm:

### Step 1:
Perform standard imports
- Import `torch` and `NumPy`.

```python
import torch
import numpy as np
```

### Step 2:
Set the random seed for NumPy and PyTorch both to `42`.

```python
np.random.seed(42)
torch.manual_seed(42)
```

### Step 3:
Create a NumPy array called `arr` that contains 6 random integers between 0 (inclusive) and 5 (exclusive).

```python
arr = np.random.randint(0,5,6)
print(arr)
```

### Step 4:
Create a tensor `x` from the array above.

```python
x=torch.tensor(arr)
print(x,x.dtype)
```

### Step 5:
Change the dtype of `x` from `int32` to `int64`.

```python
 print(x,x.dtype)
```

### Step 6:
Reshape `x` into a `3x2` tensor.

```python
x = torch.tensor(arr, dtype=torch.int64)
x = x.reshape(3, 2)
x
```

### Step 7:
Return the right-hand column of tensor `x`.

```python
right=print(x[:,1:])
```

### Step 8:
Without changing `x`, return a tensor of square values of `x`.

```python
squared_x = torch.square(x) 
squared_x
```

### Step 9:
Create a tensor `y` with the same number of elements as `x`, that can be matrix-multiplied with `x`.
- Use PyTorch directly (not NumPy) to create a tensor of random integers between 0 (inclusive) and 5 (exclusive).

```python
y=torch.randint(0,5,(2,3))
print(y)
```

### Step 10:
Find the matrix product of `x` and `y`.

```python
print(torch.mm(x,y))
```

## Output:
i) Import and set up PyTorch and NumPy.

<img width="360" height="99" alt="Screenshot 2025-08-11 225417" src="https://github.com/user-attachments/assets/d8464180-7ce0-426e-b298-5d8cc96622b4" />


ii) Create and manipulate tensors.

![image](https://github.com/user-attachments/assets/d8484961-8ac8-4bb7-85f3-6ba09dcba339)




![image](https://github.com/user-attachments/assets/be1b9dd5-9df2-4de6-bf7f-2d36a1f353d5)





![image](https://github.com/user-attachments/assets/c1321dc7-f9c1-4576-8a3b-80548c8b5182)




![image](https://github.com/user-attachments/assets/1613f9e5-5859-4916-82f3-ac6c5a4fe3b9)


iii) Perform matrix operations.



![image](https://github.com/user-attachments/assets/b6d1fe49-9d56-4558-8d68-c0c91bea9903)




![image](https://github.com/user-attachments/assets/a5f34554-155f-439b-92ed-559b1153f5e5)




![image](https://github.com/user-attachments/assets/16545d27-6f86-4952-90c6-8ae2c7b03c45)



![image](https://github.com/user-attachments/assets/2521aff3-434b-4a83-a381-cdafe7d44a0f)



![image](https://github.com/user-attachments/assets/a8ff1fba-0783-4549-b6a7-600c357df005)



## Result:
Thus, the PyTorch tensor operations, including reshaping, dtype conversion, and matrix multiplication, were successfully performed using the Python program.
