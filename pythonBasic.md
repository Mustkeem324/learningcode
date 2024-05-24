# Python Basics Tutorial

## Introduction
Python is a high-level, interpreted programming language known for its simplicity and readability. It's widely used in various fields, including web development, data science, artificial intelligence, and more.

## Setting Up Python
1. **Download and Install Python**:
   - Visit [python.org](https://www.python.org/downloads/) and download the latest version.
   - Follow the installation instructions for your operating system.
   - Ensure you check the option to add Python to your system PATH during installation.

2. **Verify Installation**:
   Open a terminal (or command prompt) and type:
   ```sh
   python --version
   ```
   This should display the installed Python version.

3. **Install an IDE or Text Editor**:
   - Popular choices include PyCharm, VS Code, Sublime Text, and Jupyter Notebook.

## Basic Syntax and Data Types

### Hello, World!
Let's start with a simple "Hello, World!" program:
```python
print("Hello, World!")
```

### Comments
Comments are ignored by the interpreter and are used to explain code.
```python
# This is a single-line comment

"""
This is a 
multi-line comment
"""
```

### Variables
Variables are used to store data.
```python
x = 5           # Integer
y = 3.14        # Float
name = "Alice"  # String
is_active = True # Boolean
```

### Data Types
1. **Numbers**:
   - Integers: `int`
   - Floating-point: `float`
2. **Strings**:
   ```python
   greeting = "Hello"
   ```
3. **Booleans**:
   ```python
   is_active = True
   ```

### Type Casting
Convert one data type to another.
```python
x = int("10")     # Converts string to integer
y = float("3.14") # Converts string to float
z = str(5)        # Converts integer to string
```

## Operators

### Arithmetic Operators
```python
a = 10
b = 3

print(a + b)  # Addition
print(a - b)  # Subtraction
print(a * b)  # Multiplication
print(a / b)  # Division
print(a % b)  # Modulus
print(a ** b) # Exponentiation
print(a // b) # Floor Division
```

### Comparison Operators
```python
print(a == b)  # Equal
print(a != b)  # Not equal
print(a > b)   # Greater than
print(a < b)   # Less than
print(a >= b)  # Greater than or equal to
print(a <= b)  # Less than or equal to
```

### Logical Operators
```python
print(a > 5 and b < 5)  # Logical AND
print(a > 5 or b > 5)   # Logical OR
print(not(a > 5))       # Logical NOT
```

## Control Flow

### Conditional Statements
```python
x = 10

if x > 0:
    print("x is positive")
elif x == 0:
    print("x is zero")
else:
    print("x is negative")
```

### Loops

#### `for` Loop
```python
for i in range(5):
    print(i)  # Prints 0 to 4
```

#### `while` Loop
```python
count = 0
while count < 5:
    print(count)
    count += 1
```

### `break` and `continue`
```python
for i in range(10):
    if i == 5:
        break  # Exits the loop
    print(i)

for i in range(10):
    if i % 2 == 0:
        continue  # Skips to the next iteration
    print(i)
```

## Functions
Functions are reusable blocks of code.
```python
def greet(name):
    print("Hello, " + name)

greet("Alice")
```

### Return Statement
```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)
```

## Data Structures

### Lists
Lists are ordered, mutable collections.
```python
fruits = ["apple", "banana", "cherry"]
print(fruits[0])  # Access element
fruits.append("orange")  # Add element
print(fruits)
```

### Tuples
Tuples are ordered, immutable collections.
```python
point = (10, 20)
print(point[0])
```

### Sets
Sets are unordered collections with no duplicate elements.
```python
numbers = {1, 2, 3, 4, 4}
print(numbers)
```

### Dictionaries
Dictionaries store key-value pairs.
```python
person = {"name": "Alice", "age": 25}
print(person["name"])
person["age"] = 26  # Update value
```

## Modules and Packages

### Importing Modules
```python
import math
print(math.sqrt(16))

from math import pi
print(pi)
```

## File Handling
```python
# Writing to a file
with open("test.txt", "w") as file:
    file.write("Hello, World!")

# Reading from a file
with open("test.txt", "r") as file:
    content = file.read()
    print(content)
```

## Exception Handling
```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
finally:
    print("This will always execute")
```

## Object-Oriented Programming (OOP)

### Classes and Objects
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        print("Hello, my name is " + self.name)

# Create an object
person1 = Person("Alice", 25)
person1.greet()
```

### Inheritance
```python
class Employee(Person):
    def __init__(self, name, age, employee_id):
        super().__init__(name, age)
        self.employee_id = employee_id

employee1 = Employee("Bob", 30, "E123")
employee1.greet()
```

## Conclusion
This tutorial covers the basics of Python programming. With these fundamentals, you can start exploring more advanced topics and building your own projects. Happy coding!
