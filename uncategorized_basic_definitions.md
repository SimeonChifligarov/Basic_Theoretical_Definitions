
# Data type
	[...]

 - In Python:
Numeric Types: int, float, complex
String
List, Set, Tuple, Dictionary
Boolean

# Boolean
 - represents a logical entity and can have two values: True and False

# None keyword
 - There are two ways to check if a variable is None
	- if null_variable is None:  # (1)
	- if null_variable == None:  # (2)

# operators
An operator in a programming language is a symbol that tells the compiler or interpreter
to perform specific mathematical, relational or logical operation and produce final result.
 - https://www.tutorialspoint.com/computer_programming/computer_programming_operators.htm

# operands
In computers, an operand is the part of a computer instruction that specifies data
that is to be operating on or manipulated and, by extension, the data itself
An operand is an object of a mathematical or other operation.
These are commonly expressed in computer programming as constants or variables.

# Operator Overloading
 - An operator behaves differently based on the type of the operands
    - e.g., operator "+" is used to add two integers as well as join two strings and merge two lists
    - It is overloaded by int class, str class and list class


# Python built-in functions
 The Python interpreter has a number of functions and types built into it that are always available.
 - https://docs.python.org/3/library/functions.html#ascii

# Python keywords
 - https://www.w3schools.com/python/python_ref_keywords.asp (33)

# Predicate
 - Predicate in general meaning is a statement about something that is either true or false.
In programming, predicates represent single argument functions that return a boolean value.



# Generator expression
	[...]

 - A generator comprehension - single-line specification for defining a generator in Python.

# io module
 - The io module provides Python's main facilities for dealing with various types of I/O.
	[...]

 - I/O (input/output) describes any operation, program, or device that transfers data to or from a computer.
    Typical I/O devices are printers, hard disks, keyboards, and mouses.

# PIP
Package Management System (PIP)
External modules are downloaded from the internet by using pip

Pip is a recursive acronym that can stand for either "Pip Installs Packages" or "Pip Installs Python".
Alternatively, pip stands for "preferred installer program".
Python 3.4 and later include pip (pip3 for Python 3) by default.

А Requirements.txt file is just a list of pip install arguments placed in a file


# Errors
	[...]

 - SyntaxError - A certain statement is not in accordance with the prescribed usage

 - IndexError is thrown (RAISED) when trying to access an item at an invalid index
 - KeyError is thrown when a key is not found
 - TypeError is thrown when an operation or function is applied to an object of an inappropriate type  # '2'+2
 - ValueError is thrown when a function's argument is of an inappropriate type  # int('xyz')
 - NameError is thrown when an object could not be found  # NameError: name 'age' is not defined
