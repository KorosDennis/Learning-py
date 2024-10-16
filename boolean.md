***Booleans*** are a common type in Python. Their value can only ever be one of two things: true or false. Understanding how to use Boolean values is critical, because you need them to write conditional logic.

**What will you learn?**

By the end of this module, you'll be able to:

    1. Run code under various conditions by using  `if, else, and elif` statements.
    2. Combine conditional logic and create more complex conditions by using and and or operators.

    > This module teaches you how to use conditional logic to create decision-driven programs.


**Write 'if' statements**


To express conditional logic in Python, you use if statements. When you're writing an if statement, you're relying on another concept we cover in this module, mathematical operators. Python supports the common logic operators from math: equals, not equals, less than, less than or equal to, greater than, and greater than or equal to. You're probably used to seeing these operators displayed using symbols, which is how they’re represented in Python, too.

    Equals: a == b
    Not Equals: a != b
    Less than: a < b
    Less than or equal to: a <= b
    Greater than: a > b
    Greater than or equal to: a >= b

### Test expressions

You need to use an if statement to run code only if a certain condition is satisfied. The first thing you do when you write an if statement is to check the condition by using a test expression. You then determine whether the statement evaluates to True or False. If it's True, the next indented code block is run:
Python

```python
a = 97
```
```python
b = 55
```
```python
 # test expression
 ```
```python
if a < b:
```
```python
    # statement to be run
 ```

```python
    print(b)
```

In this example, a < b is the test expression. The program evaluates the test expression and then runs the code within the if statement only if the test expression is True. If you evaluate the expression, you know that it's False, so any code you write in the if statement won't be run.


### Write if statements

You use an if statement if you want to run code only if a certain condition is satisfied. The syntax of an if statement is always:

```python
if test_expression:
```
  statement(s) to be run

For example:

```python
a = 93
b = 27
if a >= b:
    print(a)

Output: 93
```

In Python, the body of an if statement must be indented. Any code following a test expression that isn't indented will always be run:
```Python

a = 24
b = 44
if a <= 0:
    print(a)
print(b)

Output: 44
```

In this example, the output is 44 because the test expression is False and the print(b) statement isn't indented at the same level as the if statement.


### What are 'else' and 'elif' statements 

What if you also want your program to run a piece of code when your test expression is False? Or what if you want to include another test expression? Python has other keywords you can use to make more complex if statements, else and elif. When you use if, else, and elif in combination, you can write complex programs with multiple test expressions and statements to run.
Work with else

You know that when you use an if statement, the body of the program will run only if the test expression is True. To add more code that will run when your test expression is False, you need to add an else statement.

Let's adapt an example from the previous section:
```Python

a = 27
b = 93
if a >= b:
    print(a)
```

In this example, if a isn't greater than or equal to b, nothing happens. Let's say you want to instead print b if the test expression is False:

```Python

a = 27
b = 93
if a >= b:
    print(a)
else:
    print(b)

Output: 93
```

If the test expression is False, the code in the body of the if statement is skipped, and the program continues running from the else statement. The syntax of an if/else statement is always:
```Python

if test_expression:
    # statement(s) to be run
else:
    # statement(s) to be run
```

### Work with elif

In Python, the keyword elif is short for else if. Using elif statements enables you to add multiple test expressions to your program. These statements run in the order in which they're written, so your program will enter an elif statement only if the first if statement is False. For example:

```Python

a = 27
b = 93
if a <= b:
    print("a is less than or equal to b")
elif a == b:
    print("a is equal to b")

Output: a is less than or equal to b
```

In this variation, the elif statement in the block of code won't run, because the if statement is True.

The syntax of an if/elif statement is:
```Python

if test_expression:
    # statement(s) to be run
elif test_expression:
    # statement(s) to be run

Combine if, elif, and else statements

You can combine if, elif, and else statements to create programs with complex conditional logic. Remember that an elif statement is run only when the if condition is false. Also note that an if block can have only one else block, but it can have multiple elif blocks.

Let's look at an example with an if, an elif and an else statement:
Python

a = 27
b = 93
if a < b:
    print("a is less than b")
elif a > b:
    print("a is greater than b")
else: 
    print ("a is equal to b")    

A code block that uses all three types of statements has the following syntax:
Python

if test_expression:
    # statement(s) to be run
elif test_expression:
    # statement(s) to be run
elif test_expression:
    # statement(s) to be run
else:
    # statement(s) to be run

Work with nested conditional logic

Python also supports nested conditional logic, meaning that you can nest if, elif, and else statements to create even more complex programs. To nest conditions, indent the inner conditions, and everything at the same level of indentation will be run in the same code block:
Python

a = 16
b = 25
c = 27
if a > b:
    if b > c:
        print ("a is greater than b and b is greater than c")
    else: 
        print ("a is greater than b and less than c")
elif a == b:
    print ("a is equal to b")
else:
    print ("a is less than b")

This piece of code produces the output a is less than b.

Nested conditional logic follows the same rules as regular conditional logic within each code block. Here's one example of the syntax:
Python

if test_expression:
    # statement(s) to be run
    if test_expression:
        # statement(s) to be run
    else: 
        # statement(s) to be run
elif test_expression:
    # statement(s) to be run
    if test_expression:
        # statement(s) to be run
    else: 
        # statement(s) to be run
else:
    # statement(s) to be run
```



### The and operator

```python 

You can also connect two test expressions by using the Boolean and operator. Both conditions in the test expression must be true for the entire test expression to evaluate to True. In any other case, the test expression is False. In the following example, the entire test expression evaluates to False, because only one of the conditions in the subexpressions is true:

a = 23
b = 34
if a == 34 and b == 34 :
    print(a+b)

a boolean expression that uses and has the following syntax:

sub-expression1 and sub-expression2
```

### The Difference between and, or
 
 o highlight the difference between the two Boolean operators, you can use a truth table. A truth table shows you what the entire test expression evaluates to based on the two subexpressions.

Here's the truth table for and:

subexpression1 	Operator 	subexpression2 	Result
   True 	     and 	       True 	     True
   True 	     and 	       False 	     False
   False 	     and 	       True 	     False
   False 	     and 	       False 	     False

Here's the truth table for or:

subexpression1 	Operator 	subexpression2 	 Result
    True 	        or 	        True 	      True
    True 	        or 	        False      	  True
    False 	        or 	        True 	      True
    False 	        or 	        False 	      False


## SUMMARY
```python
By using test expressions, otherwise known as Boolean expressions, you can conditionally run Python code. They're commonly used in Python to "make decisions" about what should happen next while a program is running. In the earlier units, you wrote test expressions as part of if, else, and elif statements, and you further fine-tuned your conditions by using the operators and and or.

Boolean expressions and statements are a key part of creating complex Python programs, where you want your code to run only under certain conditions.

Here are some of the essentials you now know about conditional logic:

    Booleans can have one of two values, True or False.
    if, else, and elif statements can be used to run code under specific conditions.
    and and or operators can be used to combine test expressions and create more complex conditions.

With these tools, you should feel ready to write more complex code blocks in Python.
```