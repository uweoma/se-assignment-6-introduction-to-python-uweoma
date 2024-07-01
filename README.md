[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15349632&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   ANS: 
   Python is a high-level, interpreted programming language known for its readability and simplicity.

   Some of the key features that makes it popular among developers are:
   - Readable and Maintainable Code: Python's syntax emphasizes readability, reducing the cost of program maintenance
   - Interpreted Language: Python is executed line by line, making debugging easier
   - Cross-Platform Compatibility: Python runs on many operating systems, including Windows, macOS, and Linux.
   - Comprehensive Standard Library: Python's extensive standard library supports many common programming tasks such as file I/O, system calls, and web development.
   - Community and Ecosystem: Python has a large and active community, contributing to a rich ecosystem of libraries and frameworks.

USE CASES ARE:
- Web Development: Frameworks like Django and Flask make web development straightforward.
- Data Science and Machine Learning: Libraries such as pandas, NumPy, and scikit-learn are widely used in data analysis and machine learning.
- Automation and Scripting: Python is often used for automating repetitive tasks.
- Software Development: Python can be used for backend development, desktop applications, and even games.
- Scientific Computing: Libraries like SciPy and Matplotlib are popular in scientific research.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   ANS:
   - Download Python Installer: Go to the official Python website and download the installer for Windows.
   - Run Installer: Open the installer and check the box that says "Add Python to PATH". Click "Install Now".
   - Verify Installation: Open Command Prompt and type python --version. You should see the installed Python version.
   - Set Up Virtual Environment:
      python -m venv myenv
      myenv\Scripts\activate


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   ANS: 
   print("Hello, World!")
   - print(): This is a built-in function in Python used to output text to the console.
   - "Hello, World!": This is a string, a sequence of characters enclosed in double quotes.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   ANS:
   - int: Integer numbers
   - float: Floating-point numbers
   - str: Strings
   - bool: Boolean values (True or False)
   - list: Ordered, mutable collections
   - tuple: Ordered, immutable collections
   - dict: Unordered collections of key-value pairs
   - set: Unordered collections of unique elements

   # Integer
   a = 10
   print(a, type(a))

   # Float
   b = 20.5
   print(b, type(b))

   # String
   c = "Hello"
   print(c, type(c))

   # Boolean
   d = True
   print(d, type(d))

   # List
   e = [1, 2, 3]
   print(e, type(e))

   # Tuple
   f = (1, 2, 3)
   print(f, type(f))

   # Dictionary
   g = {"name": "Alice", "age": 25}
   print(g, type(g))

   # Set
   h = {1, 2, 3}
   print(h, type(h))


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   ANS:
   Conditional Statements:
   Conditional statements allow you to execute code based on certain conditions using if, elif, and else

   x = 10
   if x > 5:
     print("x is greater than 5")
   else:
     print("x is not greater than 5")

   LOOPS:
   Loops are used to execute a block of code repeatedly. The main loops in Python are for and while.

   fruits = ["apple", "banana", "cherry", "mango", "orange"]
   for x in fruits:
      print(x)


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   ANS:
   Functions:
   Functions are reusable blocks of code that perform a specific task. They help in breaking down complex problems into smaller, manageable pieces.

   def add(a, b):
      return a + b

   # Calling the function
   result = add(5, 3)
   print(result)  
   # Output: 8


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   ANS:
   Differences:
   Lists: Ordered, mutable collections accessed by index.
   Dictionaries: Unordered collections of key-value pairs accessed by keys.

   - The list is a collection of index value pairs like that of the array in C++ while the dictionary is a hashed structure of the key and value pairs.
   - The list is created by placing elements in [ ] separated by commas “,” while the dictionary is created by placing elements in { } as “key”:”value”, each key-value pair is separated by commas “, “
   - The indices of the list are integers starting from 0 while the keys of the dictionary can be of any data type.

   # List
numbers = [1, 2, 3, 4, 5]
numbers.append(6)  # Adding an element
print(numbers)
print(numbers[2])  # Accessing an element by index

# Dictionary
person = {"name": "Alice", "age": 25}
person["city"] = "New York"  # Adding a key-value pair
print(person)
print(person["name"])  # Accessing a value by key


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   ANS: 
   Exception Handling:
   Exception handling allows you to handle runtime errors gracefully using try, except, and finally.

   try:
     result = 10 / 0
   except ZeroDivisionError as e:
     print("Error:", e)
   finally:
     print("This will always execute")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   ANS:
   Modules:
   Modules are files containing Python code that can be imported and used in other scripts.

   Packages:
   Packages are collections of modules organized in directories that include a special __init__.py file.

   import math

   result = math.sqrt(16)
   print(result)  
   # Output: 4.0

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    ANS:
    READING FROM A FILE:
    with open('example.txt', 'r') as file:
      content = file.read()
      print(content)
      
    WRITING TO A FILE:
    lines = ["First line", "Second line", "Third line"]
    with open('output.txt', 'w') as file:
      for line in lines:
        file.write(line + "\n")



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


