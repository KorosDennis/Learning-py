*For reading input from the keyboard, Python provides the input() function. input() reads what the user types on the keyboard and returns it as a string. Here's an example that combines input() and print() to capture a person's name and display it on the screen:*

```python
name = input ("Enter your name: ")
print (name)
```

The string passed as an argument to the input function is the prompt the user will see. In this example, you're asking the user to type their name ('Enter your name'). Once the user types a name and presses Enter, the input function will return. The function's return value is the text the user typed, and that text is assigned to the variable named name. The name variable is then used as an input or argument to the print function, which will output the name the user entered.

You can also call the input function without a parameter:
 
 ```python
 print('What is your name?')
name = input()
print(name)
```
This program will behave almost the same as the first one. The difference is that print (by default) adds a newline to the output.

# Reading numbers as Input

The input function always returns the typed value as a string (text). This choice makes sense because the user can enter whatever value they like. Even if the input is a valid number, it's still returned as a string type from the input function. For example:

```Python

x = input('Enter a number: ')
print(type(x))
```

Running this code and entering the value '5' would display <class 'str'>, even though the value itself is numeric. To turn the value into a true integer variable, you can use the int() function:

```Python

x = int(input('Enter a number: '))
print(type(x))
```

This code will output <class 'int'> for the value '5'. You can use the float function in the same way if you expect a fractional component.

# Converting number to String
