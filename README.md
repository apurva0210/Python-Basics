# Python Basics – Complete Study Guide

Welcome to my **Python Basics** repository! This repository contains beginner-friendly notes, explanations, code examples, and Jupyter Notebooks covering the fundamental concepts of Python programming.

The purpose of this repository is to develop a strong foundation in Python through practical examples and regular coding practice.

---

# 1. Introduction to Python

## What is Python?

Python is a high-level, general-purpose, interpreted programming language known for its simple syntax and readability. It allows programmers to write clear and understandable code with fewer lines compared with many other programming languages.

Python supports procedural, object-oriented, and functional programming. It is widely used in web development, data analytics, artificial intelligence, machine learning, automation, and scientific computing.

### Who Invented Python?

Python was created by **Guido van Rossum**, a Dutch programmer. He began developing Python in December 1989 at the Centrum Wiskunde & Informatica (CWI), a research institute in the Netherlands. Python's first public release, version 0.9.0, appeared in 1991.

Python was influenced by the ABC programming language, particularly its emphasis on readability and simplicity.

### Why Is It Called Python?

The name Python was inspired by the British comedy television series *Monty Python's Flying Circus*. Guido van Rossum wanted a short, distinctive, and memorable name for the language.

### History of Python

| Year | Development |
|---|---|
| 1989 | Guido van Rossum began developing Python. |
| 1991 | Python 0.9.0 was publicly released. |
| 1994 | Python 1.0 was released. |
| 2000 | Python 2.0 was released with several new language features. |
| 2001 | The Python Software Foundation (PSF) was established. |
| 2008 | Python 3.0 was released with significant language improvements. |
| Present | Python continues to evolve through community development and new releases. |

Python 3 is the modern version used for current Python development. Python 2 reached the end of its official support in 2020.

## Features of Python

1. **Simple and Readable:** Python code is easy to read and understand.
2. **Interpreted:** Python programs are executed by a Python implementation.
3. **High-Level:** Programmers do not need to manage most low-level hardware details.
4. **Dynamically Typed:** Variable types do not normally need to be declared explicitly.
5. **Object-Oriented:** Python supports classes, objects, inheritance, and other object-oriented concepts.
6. **Cross-Platform:** Python is available for Windows, Linux, and macOS.
7. **Open Source:** Python is freely available under its open-source licence.
8. **Large Standard Library:** Python provides many built-in modules for common programming tasks.
9. **Extensible:** Python can work with libraries and components written in other languages.

## Applications of Python

- Data Analytics and Data Science
- Artificial Intelligence and Machine Learning
- Web Development
- Task Automation and Scripting
- Scientific and Statistical Computing
- Software Testing
- Desktop Application Development
- Natural Language Processing
- Computer Vision

## First Python Program

```python
print("Hello, World!")
```

**Output:**

```text
Hello, World!
```

The `print()` function displays information on the screen. In this example, the text `"Hello, World!"` is a string.

---

# 2. Python Syntax and Semantics

## What Is Syntax?

Syntax refers to the rules that determine how statements and expressions must be written in a programming language.

## What Is Semantics?

Semantics refers to the meaning of a statement and the behaviour it produces when executed.

### Example

```python
a = 10
b = 20
print(a + b)
```

**Output:**

```text
30
```

The syntax defines how the statements are written, while the semantics explains their meaning: two values are assigned to variables, added together, and displayed.

## Important Syntax Rules

### 1. Indentation

Indentation is the whitespace at the beginning of a line. Python uses indentation to define code blocks. Four spaces are the standard convention.

```python
if 10 > 5:
    print("10 is greater than 5")
```

### 2. Comments

Comments explain code and are ignored during normal execution.

```python
# This is a single-line comment
print("Learning Python")
```

### 3. Case Sensitivity

Python is case-sensitive. For example, `name` and `Name` refer to different identifiers.

```python
name = "Apurva"
Name = "Kadam"

print(name)
print(Name)
```

### 4. Variables and Assignment

The assignment operator `=` assigns a value to a variable.

```python
age = 25
print(age)
```

### 5. Colon

A colon (`:`) introduces an indented block after statements such as `if`, `for`, `while`, and `def`.

```python
for i in range(3):
    print(i)
```

### 6. Input and Output

The `input()` function accepts user input as a string, while `print()` displays output.

```python
name = input("Enter your name: ")
print("Welcome", name)
```

---

# 3. Variables and Data Types

## What Is a Variable?

A variable is a name that refers to an object or value in a program. In Python, a variable is created when a value is assigned to it.

```python
name = "Apurva"
age = 25
marks = 85.5

print(name)
print(age)
print(marks)
```

**Output:**

```text
Apurva
25
85.5
```

## Rules for Naming Variables

- A variable name must begin with a letter or an underscore.
- It cannot begin with a number.
- It may contain letters, numbers, and underscores.
- Variable names are case-sensitive.
- Python keywords cannot be used as variable names.
- Descriptive names improve code readability.

Examples:

```python
student_name = "Apurva"
total_marks = 450
_age = 25
```

## What Is a Data Type?

A data type identifies the kind of value an object represents and determines which operations can be performed on it.

### Common Python Data Types

| Data Type | Description | Example |
|---|---|---|
| `int` | Whole numbers | `age = 25` |
| `float` | Decimal numbers | `price = 99.5` |
| `complex` | Complex numbers | `z = 2 + 3j` |
| `str` | Text | `name = "Python"` |
| `bool` | Boolean values | `is_valid = True` |
| `list` | Ordered, mutable collection | `[10, 20, 30]` |
| `tuple` | Ordered, immutable collection | `(10, 20, 30)` |
| `set` | Collection of unique elements | `{10, 20, 30}` |
| `dict` | Key-value mapping | `{"name": "Apurva"}` |
| `NoneType` | Represents the absence of a value | `result = None` |

### Checking a Data Type

The `type()` function returns the type of an object.

```python
x = 100
y = 10.5
z = "Python"

print(type(x))
print(type(y))
print(type(z))
```

**Output:**

```text
<class 'int'>
<class 'float'>
<class 'str'>
```

## Type Conversion

Type conversion changes a value from one data type to another when the conversion is supported.

```python
number = "100"
converted_number = int(number)

print(converted_number + 50)
```

**Output:**

```text
150
```

Common conversion functions include `int()`, `float()`, `str()`, `list()`, and `tuple()`.

---

# 4. Operators in Python

## What Is an Operator?

An operator is a symbol or keyword used to perform an operation on values or variables.

Python supports several categories of operators.

## 4.1 Arithmetic Operators

Arithmetic operators perform mathematical calculations.

| Operator | Meaning | Example |
|---|---|---|
| `+` | Addition | `10 + 5 = 15` |
| `-` | Subtraction | `10 - 5 = 5` |
| `*` | Multiplication | `10 * 5 = 50` |
| `/` | Division | `10 / 5 = 2.0` |
| `//` | Floor division | `11 // 2 = 5` |
| `%` | Modulus (remainder) | `11 % 2 = 1` |
| `**` | Exponentiation | `2 ** 3 = 8` |

Example:

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

## 4.2 Comparison Operators

Comparison operators compare values and return a Boolean result.

- `==` — Equal to
- `!=` — Not equal to
- `>` — Greater than
- `<` — Less than
- `>=` — Greater than or equal to
- `<=` — Less than or equal to

Example:

```python
a = 10
b = 20

print(a == b)
print(a < b)
print(a != b)
```

**Output:**

```text
False
True
True
```

## 4.3 Assignment Operators

Assignment operators assign values or update an existing variable.

Examples include `=`, `+=`, `-=`, `*=`, `/=`, and `//=`.

```python
x = 10
x += 5

print(x)
```

**Output:**

```text
15
```

## 4.4 Logical Operators

Logical operators combine or reverse Boolean conditions.

- `and` — True when both conditions are true.
- `or` — True when at least one condition is true.
- `not` — Reverses a truth value.

```python
age = 25

print(age >= 18 and age <= 60)
print(age < 18 or age > 60)
print(not (age < 18))
```

## 4.5 Membership Operators

Membership operators check whether a value is present in a sequence or collection.

- `in`
- `not in`

```python
fruits = ["apple", "banana", "mango"]

print("apple" in fruits)
print("grapes" not in fruits)
```

## 4.6 Identity Operators

Identity operators check whether two references point to the same object.

- `is`
- `is not`

```python
a = None
print(a is None)
```

**Output:**

```text
True
```

Use `==` to compare values and `is` primarily when checking object identity or singleton values such as `None`.

## 4.7 Bitwise Operators

Bitwise operators work on the individual bits of integers. They include `&`, `|`, `^`, `~`, `<<`, and `>>`.

```python
a = 5
b = 3

print(a & b)
print(a | b)
```

**Output:**

```text
1
7
```

---

# 5. Conditional Statements

## What Are Conditional Statements?

Conditional statements allow a program to make decisions by evaluating conditions. Depending on the result, different blocks of code can execute.

Python provides `if`, `elif`, and `else`.

## 5.1 The `if` Statement

The `if` statement executes a block when its condition is true.

```python
age = 20

if age >= 18:
    print("Eligible to vote")
```

**Output:**

```text
Eligible to vote
```

## 5.2 The `if-else` Statement

The `else` block executes when the `if` condition is false.

```python
number = 7

if number % 2 == 0:
    print("Even number")
else:
    print("Odd number")
```

**Output:**

```text
Odd number
```

## 5.3 The `if-elif-else` Statement

The `elif` keyword checks additional conditions when preceding conditions are false.

```python
marks = 75

if marks >= 80:
    print("Grade A")
elif marks >= 60:
    print("Grade B")
elif marks >= 40:
    print("Grade C")
else:
    print("Fail")
```

**Output:**

```text
Grade B
```

## 5.4 Nested Conditional Statements

A nested conditional is a conditional statement placed inside another conditional block.

```python
age = 22
has_id = True

if age >= 18:
    if has_id:
        print("Entry allowed")
    else:
        print("ID required")
else:
    print("Entry not allowed")
```

Conditional statements are useful for validating input, assigning grades, checking eligibility, and implementing business rules.

---

# 6. Loops in Python

## What Is a Loop?

A loop repeatedly executes a block of code. Loops reduce repetition and are useful when processing sequences, performing calculations, or repeating a task until a condition changes.

Python has two main loop statements: `for` and `while`.

## 6.1 The `for` Loop

A `for` loop iterates over items in an iterable, such as a list, string, tuple, or range.

```python
for i in range(1, 6):
    print(i)
```

**Output:**

```text
1
2
3
4
5
```

The `range(1, 6)` expression generates numbers starting at 1 and stopping before 6.

### Iterating Through a List

```python
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)
```

## 6.2 The `while` Loop

A `while` loop repeats as long as its condition is true.

```python
i = 1

while i <= 5:
    print(i)
    i += 1
```

The variable is incremented on each iteration so that the loop eventually terminates.

## 6.3 Loop Control Statements

### `break`

Terminates the nearest enclosing loop.

```python
for i in range(1, 6):
    if i == 4:
        break
    print(i)
```

### `continue`

Skips the rest of the current iteration and continues with the next iteration.

```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
```

### `pass`

Acts as a placeholder when a statement is syntactically required but no action is needed yet.

```python
for i in range(3):
    pass
```

Loops are useful for processing datasets, calculating totals, searching collections, and automating repetitive work.

---

# 7. Lists, Tuples, Sets, and Dictionaries

Python provides built-in collection types for storing and organizing multiple values.

## 7.1 Lists

A list is an ordered, mutable collection that allows duplicate values. Lists are written using square brackets `[]`.

```python
fruits = ["apple", "banana", "mango"]

print(fruits[0])

fruits.append("orange")
fruits[1] = "grapes"

print(fruits)
```

**Output:**

```text
apple
['apple', 'grapes', 'mango', 'orange']
```

Common list methods:

- `append()` — Adds an item at the end.
- `insert()` — Adds an item at a specified position.
- `remove()` — Removes the first matching item.
- `pop()` — Removes and returns an item.
- `sort()` — Sorts a list in place.
- `len()` — Returns the number of items.

Lists are useful when data needs to be stored in order and modified.

## 7.2 Tuples

A tuple is an ordered, immutable collection that allows duplicate values. Tuples are usually written using parentheses `()`.

```python
numbers = (10, 20, 30, 20)

print(numbers[0])
print(numbers.count(20))
print(len(numbers))
```

**Output:**

```text
10
2
4
```

A tuple's elements cannot be reassigned. However, if a tuple contains a mutable object, that object's contents may still be changed.

Tuples are useful for fixed collections of related values.

## 7.3 Sets

A set is a collection of unique elements. Sets do not support indexing and do not guarantee a display order.

```python
numbers = {10, 20, 20, 30}

print(len(numbers))
print(20 in numbers)
```

**Output:**

```text
3
True
```

Common set operations include:

- `add()` — Adds an element.
- `remove()` — Removes an element and raises an error if it is absent.
- `discard()` — Removes an element if present.
- `union()` — Combines elements from sets.
- `intersection()` — Finds common elements.
- `difference()` — Finds elements present in one set but not the other.

Sets are useful for removing duplicates and comparing collections.

## 7.4 Dictionaries

A dictionary stores data as key-value pairs. Dictionaries are mutable and preserve insertion order in modern Python.

```python
student = {
    "name": "Apurva",
    "age": 25,
    "marks": 85
}

print(student["name"])

student["marks"] = 90
student["city"] = "Mumbai"

print(student)
```

Common dictionary methods:

- `keys()` — Returns the keys.
- `values()` — Returns the values.
- `items()` — Returns key-value pairs.
- `get()` — Retrieves a value without raising a `KeyError` for a missing key.
- `update()` — Adds or updates entries.
- `pop()` — Removes a key and returns its value.

Dictionaries are useful for representing structured information such as student records, product details, and configuration settings.

## Collection Comparison

| Feature | List | Tuple | Set | Dictionary |
|---|---|---|---|---|
| Syntax | `[]` | `()` | `{1, 2}` | `{"a": 1}` |
| Ordered | Yes | Yes | No guaranteed order | Yes |
| Mutable | Yes | No | Yes | Yes |
| Duplicates | Allowed | Allowed | Not for elements | Keys must be unique |
| Access | Index | Index | Membership | Key |

---

# 8. Functions in Python

## What Is a Function?

A function is a reusable block of code designed to perform a particular task. Functions help organize programs into smaller, manageable components and reduce code duplication.

Python provides built-in functions and allows programmers to define their own functions.

## 8.1 Defining and Calling a Function

Functions are defined using the `def` keyword.

```python
def greet():
    print("Hello, Apurva!")

greet()
```

**Output:**

```text
Hello, Apurva!
```

## 8.2 Parameters and Arguments

Parameters are names defined in a function declaration. Arguments are the values supplied when the function is called.

```python
def greet(name):
    print("Hello", name)

greet("Apurva")
```

**Output:**

```text
Hello Apurva
```

## 8.3 Return Statement

The `return` statement sends a result back to the caller.

```python
def add(a, b):
    return a + b

result = add(10, 20)
print(result)
```

**Output:**

```text
30
```

## 8.4 Default Arguments

A default argument provides a value used when the caller omits that argument.

```python
def greet(name="Guest"):
    print("Welcome", name)

greet()
greet("Apurva")
```

## 8.5 Lambda Functions

A lambda function is a small anonymous function defined using the `lambda` keyword. Its body is a single expression.

```python
square = lambda x: x * x

print(square(5))
```

**Output:**

```text
25
```

## 8.6 Scope of Variables

A local variable is defined inside a function and is generally accessible only within that function. A global variable is defined outside functions and may be accessed within them, subject to Python's scope rules.

```python
message = "Python"

def display():
    language = "Programming"
    print(message)
    print(language)

display()
```

Functions improve reusability, testing, readability, and program organization.

---

# 9. Exception Handling

## What Is an Exception?

An exception is an event raised during program execution that interrupts the normal flow of instructions. Examples include division by zero, invalid type conversion, and attempts to access a missing dictionary key.

Exception handling allows programs to respond to such errors in a controlled way.

## 9.1 The `try` and `except` Statements

The `try` block contains code that may raise an exception. The `except` block handles a matching exception.

```python
try:
    number = int(input("Enter an integer: "))
    print(number)
except ValueError:
    print("Invalid input. Enter a valid integer.")
```

If the user enters non-numeric text, Python raises a `ValueError`, which is handled by the `except` block.

## 9.2 Handling Multiple Exceptions

Different exception types can be handled separately.

```python
try:
    a = int(input("Enter the first number: "))
    b = int(input("Enter the second number: "))
    print(a / b)
except ValueError:
    print("Please enter valid integers.")
except ZeroDivisionError:
    print("Division by zero is not allowed.")
```

## 9.3 The `else` Block

The `else` block executes if the `try` block finishes without raising an exception.

```python
try:
    number = int("100")
except ValueError:
    print("Invalid number")
else:
    print("Converted successfully:", number)
```

## 9.4 The `finally` Block

The `finally` block executes whether or not an exception occurs. It is commonly used for cleanup operations.

```python
try:
    print(10 / 2)
except ZeroDivisionError:
    print("Cannot divide by zero")
finally:
    print("Execution completed")
```

## 9.5 Raising Exceptions

The `raise` statement allows a program to raise an exception explicitly.

```python
age = -1

if age < 0:
    raise ValueError("Age cannot be negative")
```

Exception handling improves program reliability and helps produce clearer error messages. Specific exceptions should generally be handled instead of catching every possible error indiscriminately.

---

# 10. Modules and Libraries

## What Is a Module?

A module is a Python file containing reusable definitions, such as functions, classes, and variables. Modules allow code to be organized into separate files and imported when needed.

## What Is a Library?

A library is a collection of reusable code that helps programmers perform specific tasks. It may contain modules and packages.

## 10.1 Importing a Module

The `import` statement makes a module available for use.

```python
import math

print(math.sqrt(25))
print(math.pi)
```

**Output:**

```text
5.0
3.141592653589793
```

## 10.2 Importing Specific Functions

The `from ... import ...` statement imports selected names.

```python
from math import factorial

print(factorial(5))
```

**Output:**

```text
120
```

## 10.3 Using an Alias

The `as` keyword assigns an alternative name to an imported module.

```python
import math as m

print(m.sqrt(16))
```

**Output:**

```text
4.0
```

## 10.4 Creating a User-Defined Module

Create a Python file named `calculator.py` containing:

```python
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b
```

In another Python file in the same directory, write:

```python
import calculator

print(calculator.add(10, 5))
print(calculator.subtract(10, 5))
```

**Output:**

```text
15
5
```

## 10.5 Common Python Libraries

| Library | Main Purpose |
|---|---|
| NumPy | Numerical calculations and multidimensional arrays |
| Pandas | Data manipulation and analysis |
| Matplotlib | Creating charts and graphs |
| Seaborn | Statistical data visualization |
| Scikit-learn | Machine learning algorithms and evaluation tools |
| TensorFlow | Machine learning and deep learning |
| Requests | Making HTTP requests |
| Flask | Building web applications and APIs |
| Django | Developing web applications |
| OpenCV | Image processing and computer vision |

## Installing Third-Party Libraries

The `pip` tool is commonly used to install third-party Python packages.

For example:

```bash
python -m pip install numpy pandas matplotlib
```

After installation, import the required library into your program.

```python
import numpy as np
import pandas as pd

numbers = np.array([10, 20, 30])
print(numbers.mean())

data = pd.DataFrame({"Marks": [70, 80, 90]})
print(data)
```

Modules and libraries make Python development more efficient by providing reusable functionality.

---

# 11. Conclusion

Python is a versatile programming language with readable syntax, a large standard library, and a wide ecosystem of third-party packages. Understanding its fundamentals is essential before moving to advanced programming and data-oriented applications.

The topics covered in this repository provide a foundation for learning:

- Programming fundamentals
- Data structures and algorithms
- Data analytics and visualization
- Machine learning and artificial intelligence
- Web development and automation

I will continue adding Jupyter Notebooks and practice examples as I complete each topic.

---

# 12. References

The following resources are used for further reading and learning.

1. [GeeksforGeeks – Python Basics](https://www.geeksforgeeks.org/python/python-basics/)
2. [GeeksforGeeks – Introduction to Python](https://www.geeksforgeeks.org/python/introduction-to-python/)
3. [GeeksforGeeks – History of Python](https://www.geeksforgeeks.org/python/history-of-python/)
4. [GeeksforGeeks – Python Crash Course](https://www.geeksforgeeks.org/python/python-crash-course/)
5. [GeeksforGeeks – Python Operators](https://www.geeksforgeeks.org/python/python-operators/)
6. [GeeksforGeeks – Python Functions](https://www.geeksforgeeks.org/python/python-functions/)
7. [GeeksforGeeks – Python Exception Handling](https://www.geeksforgeeks.org/python/python-try-except/)
8. [GeeksforGeeks – Python Modules](https://www.geeksforgeeks.org/python/python-modules/)
9. [Official Python Documentation – History and License](https://docs.python.org/3/license.html)
10. [Official Python Documentation](https://docs.python.org/3/)

*This repository is intended for educational purposes. The examples and explanations are written as learning notes, with the linked resources provided for additional study.*
**Additional Learning Resource:** The coding examples and practical exercises in this repository are based on my learning and practice, including study materials from GeeksforGeeks and Krish Naik’s Generative AI (GenAI) course.
