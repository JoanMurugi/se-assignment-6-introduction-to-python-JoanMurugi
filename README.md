[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15482943&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
Python is a high-level, interpreted programming language known for its readability, simplicity, and versatility. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming.

Key Features:

Readable and Maintainable Code: Python's clean syntax and indentation rules promote readable and maintainable code.
Comprehensive Standard Library: Python comes with a vast standard library that includes modules and packages for various tasks.
Interpreted Language: Python code is executed line by line, which makes debugging easier.
Dynamic Typing: Variable types are determined at runtime, which simplifies code writing.
Cross-Platform: Python runs on various operating systems, including Windows, macOS, and Linux.
Community Support: A large and active community provides a wealth of resources, libraries, and frameworks.
Use Cases:

Web Development: Frameworks like Django and Flask
Data Science and Machine Learning: Libraries like Pandas, NumPy, and scikit-learn
Automation and Scripting: Automating repetitive tasks and writing scripts
Software Development: Building desktop and server applications
Scientific Computing: Tools like SciPy and Matplotlib
2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   Windows:

Download Python Installer: Visit the official Python website and download the installer for Windows.
Run the Installer: Double-click the downloaded file. Ensure you check the box that says "Add Python to PATH."
Verify Installation: Open Command Prompt and type python --version. You should see the installed Python version.
Create Virtual Environment: In your project directory, run:
sh

python -m venv venv
Activate Virtual Environment:
Windows:
sh

venv\Scripts\activate

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   print("Hello, world!")
   Explanation:

print: Built-in function to output text to the console.
"Hello, World!": String to be printed.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   Basic Data Types:

int: Integer values
float: Floating-point numbers
str: Strings
bool: Boolean values (True/False)
list: Ordered, mutable collection
tuple: Ordered, immutable collection
dict: Unordered collection of key-value pairs

# Integer
x = 10
print(x, type(x))

# Float
y = 3.14
print(y, type(y))

# String
name = "Alice"
print(name, type(name))

# Boolean
is_active = True
print(is_active, type(is_active))

# List
numbers = [1, 2, 3]
print(numbers, type(numbers))

# Tuple
coordinates = (4, 5)
print(coordinates, type(coordinates))

# Dictionary
person = {"name": "Bob", "age": 25}
print(person, type(person))


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
Conditional statements allow you to execute certain blocks of code based on whether a condition is true or false. The most common conditional statement in Python is the if-else statement.
Example

age = 20

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")

Explanation:

if age >= 18: checks if the value of age is greater than or equal to 18.
If the condition is true, it prints "You are an adult."
If the condition is false, it prints "You are a minor."

Loops
Loops allow you to execute a block of code multiple times. Python has two main types of loops: for loops and while loops.

For Loop:

A for loop is used to iterate over a sequence (such as a list, tuple, dictionary, set, or string) or other iterable objects.
Example,

numbers = [1, 2, 3, 4, 5]

for num in numbers:
    print(num)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
Functions are reusable blocks of code that perform a specific task. They help in modularizing code and improving readability.

def add(a, b):
    return a + b

# Calling the function
result = add(3, 4)
print(result)  # Output: 7

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   Lists vs. Dictionaries:

List: Ordered collection, accessed by index.
Dictionary: Unordered collection, accessed by key.
# List
numbers = [1, 2, 3, 4, 5]
print(numbers[2])  # Accessing element at index 2

# Dictionary
student = {"name": "John", "age": 21, "major": "Computer Science"}
print(student["name"])  # Accessing value by key

# List operations
numbers.append(6)
print(numbers)

# Dictionary operations
student["age"] = 22
print(student)


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
Exception handling allows you to manage errors gracefully without crashing the program.

try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
finally:
    print("This block is always executed")

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
Modules and Packages:

Module: A single file containing Python code (e.g., math.py).
Package: A collection of modules in a directory.

import math

# Using a function from the math module
print(math.sqrt(16))  # Output: 4.0

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
 READING FILE   
with open("example.txt", "r") as file:
    content = file.read()
    print(content)

WRITING TO A FILE
lines = ["First line\n", "Second line\n", "Third line\n"]
with open("output.txt", "w") as file:
    file.writelines(lines)

REFERENCES

Gowrishankar, S., & Veena, A. (2018). Introduction to Python programming. Chapman and Hall/CRC.

Koopman, P., & DeVale, J. (2000). The exception handling effectiveness of POSIX operating systems. IEEE Transactions on Software Engineering, 26(9), 837-848.

Côté, C., Létourneau, D., Michaud, F., Valin, J. M., Brosseau, Y., Raievsky, C., ... & Tran, V. (2004, September). Code reusability tools for programming mobile robots. In 2004 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)(IEEE Cat. No. 04CH37566) (Vol. 2, pp. 1820-1825). IEEE.



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


