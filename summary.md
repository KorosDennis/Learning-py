# Learning-py
roadmap to learning python 

# What is Python?
Python is one of the most popular programming languages in the world. Created in the early 1990s, Python can be employed for a wide range of uses, from automating repetitive tasks and writing web apps to building machine learning models and implementing neural networks. Researchers, mathematicians, and data scientists in particular like Python because of its rich and easy to understand syntax and the wide range of open-source packages available. Packages are shared code libraries that are freely available for anyone to use.

Python has a simple, easy to learn syntax, which emphasizes readability. Applications written in Python can run on almost any computer, including those running Windows, macOS, and popular distributions of Linux. Furthermore, the ecosystem contains a rich set of development tools for writing, debugging, and publishing Python applications.

Finally, Python is supported by an active user community that is eager to help new programmers learn the Pythonic way, where you don't just get the syntax right, but use the language the way it was intended.

# Running Python Code
Python is an interpreted language, which reduces the edit-test-debug cycle because there's no compilation step required. In order to run Python apps, you need a runtime environment/interpreter to execute the code.

Most of the runtime environments support two ways to execute Python code:

    Interactive mode: In this mode, each command you type is interpreted and executed immediately, and you see the results each time you press ENTER. The interactive mode is the default mode if you don't pass a filename to the interpreter.
    Script mode: In script mode, you put a set of Python statements into a text file with a .py extension. You then run the python interpreter and point it at the file. The program is executed line by line, and the output is displayed. There's no compilation step, as shown in the following diagram:

Diagram showing the execution of a .py file through the Python interpreter. 
 ![alt text][https://learn.microsoft.com/en-us/training/modules/intro-to-python/media/2-python-steps.png]



[def]: 2-python-steps.png

# *Interactive Help Console*
f you don't pass an argument to the help function, Python will start an interactive help.

You enter the interactive help console by typing help(). This command will list some basic instructions on how to use the help system.

From here, you can just type in the element you're interested in. For example, by typing string you'll get information about the topic string, which looks something like this:

Output 
Help on module string:

NAME
    string - A collection of string constants.

MODULE REFERENCE
    https://docs.python.org/3.9/library/string
    
    The following documentation is automatically generated from the Python
    source files.  It may be incomplete, incorrect or include features that
    are considered implementation detail and may vary between Python
    implementations.  When in doubt, consult the module reference at the
    location listed above.

    
# Variables and basic data types in Python

  _*Variables*_ are one of the fundamental building blocks of programs written in Python. Variables hold data in memory. They have names, and they can be referenced by those names. Variables also have types, which specify what type of data they can store (such as string and integer), and they can be used in expressions that use operators (such as + and -) to manipulate their values.
# *Variables*

In Python, a *variable* is declared and assigned a value using the assignment operator =. The variable is on the left-hand side of the operator, and the value being assigned—which can be an expression such as 2 + 2 and can even include other variables—is on the right-hand side. For example:

# Python

```python
x = 1         # assign variable x the value 1
```
```python
y = x + 5     # assign variable y the value of x plus 5
```
```python
z = y         # assign variable z the value of y
```

These examples assign numbers to variables, but numbers are just one of several data types Python supports. Notice there's no type declared for the variables. Python is a dynamically typed language, meaning the variable type is determined by the data assigned to it. In the previous examples, the x, y, and z variables are integer types, capable of storing positive and negative whole numbers.

Variable names are case sensitive and can use any letter, number, and the underscore (_) character. However, they can't start with a number.
Working with numbers

Most programs manipulate numbers. Computers treat integer numbers and decimal numbers differently. Consider the following code:
Python

```python
x = 1       # integer
```
```python
x = 1.0     # decimal (floating point)
```

Python creates integers from a built-in data type called int, and decimals (floating-point numbers) as instances of float. Python's built-in type() function returns a variable's data type. The following code outputs data types:
Python

x = 1
print(type(x)) # outputs: <class 'int'>

x = 1.0
print(type(x)) # outputs: <class 'float'>

The addition of the .0 to the end of 1 makes a large difference in how the programming language treats a value. The data type impacts how the value is stored in memory, how the processor (CPU) handles the data when evaluating expressions, how the data relates to other data, and what kinds operations you can perform with it.
Working with booleans

Another common data type is the **Boolean type**, which holds the value True or False:
Python

x = True
print(type(x)) # outputs: <class 'bool'>

Internally, bool is treated as a special type of integer. Technically, True has a value of 1 and False has a value of 0. Typically, Booleans aren't used to perform mathematical operations; rather, they're used to make decisions and perform branching. Nevertheless, it's interesting to understand the relationship between types. Many types are nothing more than specialized versions of more general types. Integers are a subset of floating point numbers, and Booleans are a subset of integers.
Working with strings

Along with numbers, strings are among the most commonly used data types. A string is a collection of zero or more characters. Strings are commonly declared using single quotation marks, but you can also use double quotation marks:
Python

x = 'This is a string'
```python
print(x) # outputs: This is a string
```
print(type(x)) # outputs: <class 'str'>
y = "This is also a string"

You can add strings to other strings—an operation known as "concatenation"—with the same + operator that adds two numbers:
Python

```python
x = 'Hello' + ' ' + 'World!'
```
```python
print(x) # outputs: Hello World!
```

You learn more about strings in another lesson, including how to parse them and how to manipulate them in various ways. You also learn about other important data types such as lists, which store collections of data and are frequently used to hold collections of strings.
Print to the console

In Python, the print function, which is one of more than 60 functions built into the language, outputs text to the screen.

The following statement displays "Hello World!" on the screen:
**Python**

```python
print('Hello World!')
```

The argument passed to print is a string, which is one of the fundamental data types in Python used to store and manage text. By default, print outputs a newline character at the end of the line, so that a subsequent call to print starts on the next line.