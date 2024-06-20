[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15307454&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is a high-level, interpreted programming language known for its readability and simplicity. It was created by Guido van Rossum and first released in 1991. Python's design philosophy emphasizes code readability and its syntax allows programmers to express concepts in fewer lines of code.

Key Features
Readable and Maintainable Code: Python's clean syntax and indentation make it easy to read and maintain.
Extensive Standard Library: Python's extensive standard library supports many common programming tasks such as file I/O, system calls, and internet protocols.
Interpreted Language: Python is an interpreted language, which means code is executed line-by-line, making debugging easier.
Dynamic Typing: Variables in Python do not require an explicit declaration to reserve memory space, as the allocation happens automatically when a value is assigned to a variable.
Portability: Python code can run on any operating system without requiring modification.
Extensive Support for Integration: Python integrates well with other languages and technologies like C, C++, Java, and web services.
Large Community and Ecosystem: Python has a large and active community that contributes to a rich ecosystem of libraries and frameworks.
Use Cases
Web Development: Using frameworks like Django and Flask.
Data Science and Machine Learning: Libraries such as NumPy, pandas, and TensorFlow.
Automation and Scripting: Automating repetitive tasks.
Software Development: Building applications with robust backends.
Game Development: Using libraries like Pygame.
Scientific Computing: Libraries such as SciPy and Matplotlib.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

My OS is windows:
Download Python Installer:
Go to the official Python website (https://www.python.org).
Download the latest version for Windows.

Run the Installer:
Double-click the downloaded file.
Check the box "Add Python to PATH."
Select "Install Now."

Verify Installation:
Open Command Prompt.
Type python --version and pip --version to check if Python and pip are installed correctly.

Set Up Virtual Environment:
Open Command Prompt.
Run python -m venv myenv to create a virtual environment.
Activate it with myenv\Scripts\activate.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")
Explanation:
print(): A built-in function used to output text to the console.
"Hello, World!": A string literal enclosed in double quotes.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

Basic Data Types
int: Integer numbers (e.g 1, 100)
float: Floating-point numbers (e.g 1.0, 3.14)
str: Strings (e.g., "Hello")
bool: Boolean values (e.g True, False)
list: Ordered sequence of values (e.g [1, 2, 3])
tuple: Ordered, immutable sequence of values (e.g (1, 2, 3))
dict: Unordered collection of key-value pairs (e.g {"name": "Alice", "age": 25})

Script Demonstrating Variables
# Integer
a = 10
print(a)

# Float
b = 3.14
print(b)

# String
c = "Hello, World!"
print(c)

# Boolean
d = True
print(d)

# List
e = [1, 2, 3]
print(e)

# Tuple
f = (4, 5, 6)
print(f)

# Dictionary
g = {"name": "Alice", "age": 25}
print(g)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

Conditional Statements
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")

Loops
For Loop
for i in range(5):
    print(i)

While Loop
i = 0
while i < 5:
    print(i)
    i += 1

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions are blocks of reusable code that perform a specific task. They help in breaking the program into smaller, manageable pieces and promote code reusability.

   Function Example
   def add_numbers(a, b):
    return a + b

# Calling the function
result = add_numbers(5, 3)
print(result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

List: An ordered collection of elements, indexed by position. Allows duplicate elements.
Dictionary: An unordered collection of key-value pairs. Keys must be unique.

Script demonstrating lists and dictionaries
# List
numbers = [1, 2, 3, 4, 5]
print(numbers)
numbers.append(6)
print(numbers)
numbers.remove(3)
print(numbers)

# Dictionary
person = {"name": "Alice", "age": 25, "city": "New York"}
print(person)
person["email"] = "alice@example.com"
print(person)
del person["age"]
print(person)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling allows you to manage errors gracefully without crashing the program.
   Example
   try:
    x = int(input("Enter a number: "))
    y = 10 / x
    print(y)
except ZeroDivisionError:
    print("Cannot divide by zero!")
except ValueError:
    print("Invalid input!")
finally:
    print("Execution completed.")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

Module: A file containing Python code that can be imported and used in another script.
Package: A collection of modules organized in directories.
Importing and using a math module
import math

# Using functions from the math module
print(math.sqrt(16))
print(math.pi)


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    Reading from a File
    with open('example.txt', 'r') as file:
    content = file.read()
    print(content)

    Writing to a File
    lines = ["Hello, World!", "This is a file.", "Writing to it."]

    with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + '\n')


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


