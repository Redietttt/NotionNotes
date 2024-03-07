# built in function py

```python
numbers = [3,4,54,67,23,54,65,44]

square_value =[]
def square_list(list_element):
 for number in list_element:
  square_value.append(number* number)
  print(square_value)

square_list(numbers)
```

this  code has an output of

[9, 16, 2916, 4489, 529, 2916, 4225, 1936]

lambda

```python
check = lambda number: 'even number' if number % 2==0 else 'odd number’ 
print(check(7))
```

this checks if its odd or even

```python
square = lambda number: number * number
print(square(5))
```

this gets the squared number

```python
new_value =filter(lambda number: True if number%2==0 else False, numbers)

print(list(new_value))
```

and this results … [4, 54, 54, 44]

### **`print()`**

Prints the specified message or value to the standard output (usually the console).

```python
pythonCopy code
print('Hello, world!')

```

### **`len()`**

Returns the length of the specified iterable object (e.g., string, list, tuple).

```python
pythonCopy code
my_list = [1, 2, 3, 4, 5]
print(len(my_list))  # Output: 5

```

### **`type()`**

Returns the data type of the specified object.

```python
pythonCopy code
num = 10
print(type(num))  # Output: <class 'int'>

```

### **`input()`**

Reads input from the user through the console.

```python
pythonCopy code
name = input('Enter your name: ')
print('Hello,', name)

```

### **`range()`**

Generates a sequence of numbers within a specified range.

```python
pythonCopy code
for i in range(5):
    print(i)  # Output: 0 1 2 3 4

```

### **`str()`, `int()`, `float()`**

Converts the specified value to a string, integer, or floating-point number, respectively.

```python
pythonCopy code
num_str = '10'
num_int = int(num_str)
print(num_int)  # Output: 10

```

### **`list()`, `tuple()`, `set()`**

Converts the specified iterable object to a list, tuple, or set, respectively.

```python
pythonCopy code
my_tuple = (1, 2, 3)
my_list = list(my_tuple)
print(my_list)  # Output: [1, 2, 3]

```

### **`max()`, `min()`, `sum()`**

Returns the maximum, minimum, or sum of the elements in the specified iterable object.

```python
pythonCopy code
numbers = [5, 10, 3, 8]
print(max(numbers))  # Output: 10
print(min(numbers))  # Output: 3
print(sum(numbers))  # Output: 26

```

### **`sorted()`, `reversed()`**

Returns a sorted or reversed version of the specified iterable object.

```python
pythonCopy code
numbers = [5, 2, 8, 1]
sorted_numbers = sorted(numbers)
print(sorted_numbers)  # Output: [1, 2, 5, 8]

```