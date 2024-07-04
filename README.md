[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15343911&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is a powerful and versetile programming language that is widely used. It is relatively easy to read and write making it perfect for beginners to learn. It is used in fields such as data science, wed development, automation and many others.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   First go to Python.org and click on download the latest version for windows (If you are using windows). After downloading the installer, locate it and run it. Follow the wizard's instructions. After completing confirm if the installation was successful by running python --version on your terminal.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   print("Hello, World!")
   print -is a build-in function used to output text or other values to the console. It displays Hello, World! in the console.
   "Hello, World!" -Is a string. A string is a sequence of characters enclosed in quotes.
   Parentheses () -are used to pass arguments to the print function.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   Integers (int): Whole numbers, positive or negative, without decimals. x = 1 or x = -3
   Floating-point numbers (float): Numbers with a decimal point or in exponential form. x = 0.89 or x = 5y7 
   Strings (str): Ordered sequences of characters enclosed in quotes. x = "Hello" or x = 'world'
   Booleans (bool): Logical values indicating True or False. x = true or x = false
   Lists (list): Ordered, mutable collections of elements, which can be of different data types. X = [1,"yes",0.9]
   Tuples (tuple): Ordered, immutable collections of elements. x = (1, 2.5, "hello")
   Dictionaries (dict): Unordered collections of key-value pairs. x = {"name": "Alice", "age": 25}
   Sets (set): Unordered collections of unique elements. x = {1, 2, 3}

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   Conditional Statements - allows you to execute a certain command based on whether a condition is true or false. 

   x = "red"
   if x = "blue" :
      print("The sky is blue.")
   else:
      print("That is not the color of the sky.")

   For example, we can check if the input (x) is color "blue". If the condition is true we will print "The sky is blue" . If the condition is not meet we will print out "That is not the color of the sky".
   Loops - allows you to run a block of code continuously until the condition is meet.

   fruits = ["Apple","Banana","Orange","Mango"]

   for fruit in fruits:
      print(fruit)
   
   In the example above, the 'for' loop iterates through the each element in the array 'friuts' and prints out each element.   


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   Functions are a block of reusable code that performs a specific task. They help in organizing code and reduce repetition in the code.

   def add_two_numbers(x,y):
      return x + y

   #how to call a function
   result = add_two_numbers(1,2)
   print(result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   Lists are collection of elements while a dictionary contains sets of key-value pairs. Lists can have duplicates while in dictionaries the key should be unique.

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   Exception handling in Python is a mechanism to catch and handle runtime errors, ensuring that the program can handle unexpected situations gracefully without crashing.

   def divide_numbers(x, y):
      try:
         result = x / y
      except ZeroDivisionError:
         print("Error: Division by zero is not allowed.")
         result = None
      except TypeError:
         print("Error: Both arguments must be numbers.")
         result = None
      else:
         print("Division successful.")
      finally:
         print("Execution of try-except block completed.")
      return result


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   Modules and packages are mechanisms to organize and reuse code in Python. A module is a single file containing Python code that can be imported and udes in other Python scripts. Pacj=kages is a collection of modules organized in directories that include a special '__init__.py' file.

   #Calculate the square root of a number
   import math

   num = 16
   sqrt_num = math.sqrt(num)
   print(f"The square root of {num} is {sqrt_num}")


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

   #Reading a file in python
   def read_file(file_path):
      try:
         with open(file_path, 'r') as file:
            content = file.read()
            print(content)
   file_path = 'index.txt'
   read_file(file_path)

    you first open the file in read mode by using the file path and an ('r') at the end. Then read its content using 'file.read()' and finally print out its content to the console.The with statement ensures that the file is properly closed after its suite finishes.

    #Writing a file in python
    def write_file(file_path, strings):
      try:
         with open(file_path, 'w') as file:
            for string in strings:
               file.write(string + '\n')
            print(content)

   file_path = 'index.txt'
   strings = ['red', 'pink', 'white']
   write_file(file_path, strings)


   you first open the file in write mode ('w') .  If the file already exists, it will be overwritten; if it does not exist, it will be created. The '\n' writes each of te string in a new line.

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


