[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15378661&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
  
   - **Answer**: Python is a high-level programming language known for its simplicity and readability. It supports multiple paradigms, including procedural, object-oriented, and functional programming. Some key features include dynamic typing, automatic memory management, and a vast standard library. Python's popularity stems from its versatility and ease of use, making it suitable for various applications such as web development (Django, Flask), scientific computing (NumPy, SciPy), data analysis (Pandas), artificial intelligence and machine learning (TensorFlow, PyTorch), and automation (scripting, DevOps).

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   - 1. Download: Go to python.org and download the installer for your operating system.
     2. Run Installer: Execute the downloaded installer and follow the prompts.
     3. Verify Installation: Open a terminal (or command prompt) and type python --version. This should display the installed Python version.
     4. Set Up Virtual Environment: Install `virtualenv` using `pip install virtualenv`. Create a virtual environment with `python -m venv env`. Activate it with `.\env\Scripts\activate` on Windows.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   - ```
     # Python program to print "Hello, World!"
     print("Hello, World!")

   - `print()` is a built-in Python function used to display output.
   - `"Hello, World!"` is a string literal enclosed in double quotes.
   

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   - Data Types:
     1. Integer (int): Whole numbers (e.g., 5, -3).
     2. Float (float): Real numbers with a decimal point (e.g., 3.14, -0.5).
     3. String (str): Sequence of characters enclosed in quotes (e.g., "Hello", 'Python').
     4. Boolean (bool): Represents truth values (True or False).
     5. List (list): Ordered collection of items (e.g., [1, 2, 3]).
     6. Dictionary (dict): Key-value pairs (e.g., {"name": "John", "age": 30}).
  
   - Example Script:
     ```
     # Python script demonstrating data types and variables
     num1 = 5        # Integer variable
     num2 = 3.14     # Float variable
     message = "Hello, Python!"  # String variable
     is_valid = True  # Boolean variable

     my_list = [1, 2, 3]  # List variable
     my_dict = {"name": "Alice", "age": 25}  # Dictionary variable

     print(num1)
     print(num2)
     print(message)
     print(is_valid)
     print(my_list)
     print(my_dict)

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   - Used to iterate over a sequence of elements or execute a block of code repeatedly until a condition is met.
   - Conditional Statements (`if-else`):
   - ```
     # Example of if-else statement
     num = 10
     if num > 0:
         print("Positive number")
     else:
         print("Non-positive number")

   - Loops (`for` loop):
   - ```
     # Example of for loop
     fruits = ["apple", "banana", "cherry"]
     for fruit in fruits:
         print(fruit)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   - Functions are blocks of reusable code designed to perform a specific task. They enhance code readability, promote code reuse, and facilitate modular programming.

   ```
   # Function to calculate the sum of two numbers
   def add_numbers(a, b):
   return a + b

   # Example of calling the function
   result = add_numbers(3, 5)
   print("Sum:", result)


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   - Lists vs. Dictionaries:

     1. Lists (list): Ordered collection of items accessed by index. Elements are enclosed in square brackets ([]).
     2. Dictionaries (dict): Unordered collection of key-value pairs accessed by keys. Elements are enclosed in curly braces ({}).
    
   - Example Script:
   - ```
     # Example of lists and dictionaries in Python
     # List of numbers
     numbers = [1, 2, 3, 4, 5]

     # Dictionary of key-value pairs
     person = {"name": "John", "age": 30, "city": "New York"}

     # Accessing elements
     print(numbers[0])        # Output: 1 (first element in list)
     print(person["name"])    # Output: John (value associated with key "name")

     # Adding elements
     numbers.append(6)        # Append number 6 to the list
     person["job"] = "Engineer"  # Add a new key-value pair to the dictionary

     # Iterating through elements
     for number in numbers:
         print(number)

     for key, value in person.items():
         print(key, ":", value)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   - Exception handling is a mechanism to handle runtime errors gracefully, preventing the program from crashing.
   - Example Script:
   - ```
     # Example of exception handling in Python
     try:
         num = int(input("Enter a number: "))
         result = 10 / num
         print("Result:", result)
     except ZeroDivisionError:
         print("Error: Division by zero!")
     except ValueError:
         print("Error: Invalid input! Please enter a valid number.")
     finally:
         print("Execution complete.")

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   - Modules and Packages:
     - Modules: Python files containing Python definitions, functions, and statements.
     - Packages: Collection of modules grouped together.
    
   - Example Using `math` Module:
   - ```
     # Example of using the math module in Python
     import math

     # Calculate square root
     num = 16
     sqrt_num = math.sqrt(num)
     print("Square root of", num, "is", sqrt_num)

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    - Reading from a File:
    - ```
      # Example of reading from a file
      file_path = "sample.txt"

      with open(file_path, 'r') as file:
          content = file.read()
          print("File Content:")
          print(content)

    - Writing to a File:
    - ```
      # Example of writing to a file
      file_path = "output.txt"
      lines_to_write = ["Line 1\n", "Line 2\n", "Line 3\n"]

      with open(file_path, 'w') as file:
          file.writelines(lines_to_write)

      print("Data written to", file_path)


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


