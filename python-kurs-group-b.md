author: Sondre Halvorsen
id: programming-with-python
summary: This course is meant as an introduction to programming using Python
status: draft
feedback link:

# Learn Programing with Python!

## About this Course
Duration: 5:00

![Python Logo](resources/python-logo-generic.svg)

This course will walk you through the basic concepts of Programming using the Python programming language.

Great online course/book for practical use of Python: [automate the boring stuff](https://automatetheboringstuff.com/)

A more academic deep dive course in programming with Python: [Edx](https://www.edx.org/course/computing-in-python-i-fundamentals-and-procedural-programming-2) PS: There is an option to pay to get a certificate for completing the course. This is optional! Completing the course without a certificate is free.


## Programming 1
Duration: 5:00

Programming is simply the act of entering instructions for the computer to perform. These instructions might crunch some numbers, modify text, look up information in files, or communicate with other computers over the Internet.

A program is like a:
 - Cooking recipe
 - Ikea assembly manual

But for the computer!

![Code image](resources/code_image.png)

## Programming 2
Duration: 5:00

For most people, their computer is just an appliance instead of a tool. But by learning how to program, you’ll gain access to one of the most powerful tools of the modern world, and you’ll have fun along the way. Programming isn’t brain surgery—it’s fine for amateurs to experiment and make mistakes.

All programs, written in any language uses the same basic building blocks

Her are a few of the most common:
 - "Do this; Then do that"
 - "If this condition is true, perform this action; otherwise, do that action"
 - "Do this action that number of times"
 - "Keep doing that until this condition is true"

![Blocks image](resources/blocks2.png)

## Programming 3
Duration: 5:00

All programming no matter the language follows three simple steps.

1. Write code as text in a editor

2. Compile the code to machine code the computer can run

3. Run the machine code on the computer

Different programming language package these steps differently. But the steps remain the same.

 ![Python code process](resources/python-i.png)


## Python
Python is a clear and powerful object-oriented programming language, comparable to Perl, Ruby, Scheme, or Java.


Developed by Guido van Rossum

## Installation
Duration: 10:00

### Windows
 - Go to https://www.python.org/downloads/
 - Download the latest version of Python (as of this course being written: Python 3.7.2)
 - Run the installer
 - enable PATH
 ![Python Installer image](resources/python_win_install_checkbox.png)
 - click [Install now]

Test that Python is properly installed by running
```bash
python --version
```
in a CMD/Powershell shell.
In case of errors reference the - Using Python on Windows page: [link](https://docs.python.org/3/using/windows.html)

### Linux

Ubuntu
```bash
sudo apt-get update
sudo apt-get install python3.7
python3 --version
```

### Mac

On macOS, the best way to install Python 3 is to use Homebrew. Not familiar with homebrew? [link](https://brew.sh/)

[tutorial to install homebrew and python](https://wsvincent.com/install-python3-mac/)

```bash
brew install python3
```

Verify installation

```bash
python3 --version
```


## Table-Of-Contents
Duration: 1:00

 There are several tools installed with the Python interpreter. Here are some of them:


| Tool      | Description  |
| ------------- |:-------------:|
| python interpreter     | The python interpreter. The executable that can be called directly from the command line prompt/terminal to start a new interactive python session (REPL) or to run python modules/files/packages |
| pip     | The Python package manager. The official Python package manager. Lets the user download and manage third-party packages hosted on the Python package index (PyPI)      | 
| IDLE | IDLE is Python’s Integrated Development and Learning Environment. Its a Python IDE for and by Python | 
| pydoc| The pydoc module automatically generates documentation from Python modules. | 




## Development Tools

Python can be used and developed with using only a basic text editor and the python interpreter. But for larger and more complex projects there is a benefit to use purpose built tools for Python development.

VSCODE is a good and free text editor: [link](https://code.visualstudio.com/)

![vscode image](resources/vscode.png)


## Python a overview
Duration: 2:00


Objects are Python’s abstraction for data. All data in a Python program is represented by objects or by relations between objects.

 - Python is strongly typed and dynamically typed.

 - Python is a general purpose programming language. It is not the best choice for time critical or memory constrained tasks.

 - Python is really a compiled programming language, but it acts as a interpreted language.

 - There exist different implementation of Python. The most common, and the one we will use in this course is CPython.

 - Python comes with "Batteries included", meaning Python comes with a feature rich standard library.



## Python 2 and Python 3
Duration: 1:00

Python has two main versions. Python 2 and Python 3. Python 3 is the newest, but it has struggled with adoption for some time. Python 3 has as of 2018 taken the mantle as the main version from Python 2.

Practically this means that new Python packages and application will in most cases be written in Python 3. 

### Python 2 end of life is january 1 2020.

![Python 2 to Python 3](resources/2_to_3.jpeg)


## Python Basics
Duration: 5:00


Arithmetic

#### In the REPL try:

adding
```python
 2 + 2
```
subtracting
```python
 3 - 2
```

multiplying
```python
 4 * 2
```

dividing
```python
 4 / 2
```

exponent
```python
 4 ** 3
```

modulus
```python
 4 % 2
```

integer division
```python
 3 // 2
```

## On errors
Duration: 1:00

#### Errors are Okay!

Programs will crash if they contain code the computer can’t understand, which will cause Python to show an error message. An error message won’t break your computer, though, so don’t be afraid to make mistakes. A crash just means the program stopped running unexpectedly.

## Python Objects and Types
Duration: 5:00

In a typical Python program there is a lot less dumb grunt work than in program implemented in other languages. Python provides powerful object types built into the language. There is less of a need to code up several functions and classes to get only the basic functionality.

#### Python built-in types

| Object Type     | Example  |
| ------------- |:-------------:|
| Numbers     | 12 , 343.34 , Decimal() |
| Strings    | "sauna", 'python' | 
| Lists| [1, "two, [ 4, 5] ]| 
| Dictionaries | {"breakfast": "eggs", "number": 1, "nested": {1: "element"}} | 
| Tuples | (1, "bacon", 13.2, ["data", 1]) | 
| Sets | set("aaaa") -> {"a"}| 
| Booleans| True, False | 
| NoneType | None | 

## Variables
Duration: 5:00

When programming you will need to store values for later use. The way we do this in Python is to give our values names we can later call to get back the value we stored in them.

#### Variable names
- It can be only one word.

- It can use only letters, numbers, and the underscore (_) character.

- It can’t begin with a number.


Creating a variable containing the integer 5
```python

my_int  = 5

```

We can then later use our variable to do some work. Note that in this case we store the result in a new variable.
```python

result = my_int * 10

```

![Python variable image](resources/python-variables.png)


## Strings
Duration: 5:00

Strings represent characters in Python and is created like this:

```python

"A string"

'Also a string'

```

You can use both " and ', to create a String.

#### Assigning a string to a variable
```python

my_string  = "My super string!"

```


## Working with Strings
Duration: 5:00

The meaning of an operator may change based on the data types of the values next to it. With Integers the + operator adds the two numbers. But when used with Strings it joins the two Strings into a new String.

```python

my_joined_string = "Hello " + "World!" 

```

But you cannot do this

```python

my_joined_string = "Hello " + 50

```
Because the two values on either side of the + operator are of different types.

Multiplying Strings and numbers on does work

```python

my_joined_string = "Hello," * 2 # 'Hello,Hello,'

```

## Python Built-in Functions
Duration: 5:00

The Python interpreter has a number of functions and types built into it that are always available.
The full list of Python built-in functions can be found here: [link](https://docs.python.org/3/library/functions.html)

### Important Built-in Functions

```python

len() # Return the length (the number of items) of an object. 

input() # The function then reads a line from input, converts it to a string

print() # Prints to stdout

bool() # returns the True or False 

help() # Invoke the built-in help system. (This function is intended for interactive use(REPL).)


```


## Writing a Python program
Duration: 5:00

A Python program is nothing more than a text file with a fancy file ending ".py". To create our own program we need to do nothing more than write Python code in a text file and run the file with the Python interpreter.

This will run the code written in the file "my_program.py"
```
python my_program.py 
```


## Exercise 1
Duration: 10:00

It is time to write your first Python program!

1. Create a new file in any text editor

2. Paste in the following Python code:

```python
print("Welcome to my program!")
user_age = input("Please enter your age")
user_name = input("Please enter your name")

print("Thank you!")
print("Your name is: " + user_name + " and your age is: " + str(user_age))

```

3. Save the file with the name: ```my_first_program.py```

4. Open a Command Prompt (CMD/Terminal)
5. Navigate to the folder where you saved the file
6. run the program ``` python my_first_program.py```


## Converting between types
Duration: 5:00

Every variable in your Python program has a type. Python is dynamically typed so the type and value of the thing a variable points to can change, but the value it points to will always have a type.

#### We can convert between built-in types with the built-in type conversion functions:

```python

str()

```


```python

int()

```


```python

float()

```



## Exercise 2
Duration: 10:00

Create a program that asks a user for two numbers.
Print the numbers back to the user on a single line.

 Hint: str() will come in handy here!


## Flow Control
 Duration: 5:00

 Control flow is the mechanisms a programmer uses to change what the program should do based on the state of the program.


![Control Flow image](resources/controll_flow2.png)

But before you learn about flow control statements, you first need to learn how to represent those yes and no options, and you need to understand how to write those branching points as Python code.


## Boolean
Duration: 5:00

Integers and Float represent numbers. String represent characters and text. Boolean represent true and false. Those two only!

Example
```python
is_true = True

is_false = False

```

## Comparison
Duration: 5:00

| Operator    | Meaning  |
| ------------- |:-------------:|
| ==     | Equal to |
| !=    | Not equal to | 
| < | Less than | 
| > | Greater than | 
| <= | Less than or equal to | 
| >= | Greater than or equal to| 

These operators evaluate to True or False depending on what is on either side of the operator.


Example
```python
10 == 10 # True
10 == 11 # False
```

```python
10 != 10 # False
10 != 11 # True
```


## Boolean Operators
Duration: 5:00

The three Boolean operators (and, or, and not) are used to compare Boolean values.

and
```python

True and False # False
True and True # True

```

or
```python

True or False # True
True or True # True
False or False  # False
```


## not Operator
Duration: 5:00

Unlike and and or, the not operator operates on only one Boolean value (or expression). The not operator simply evaluates to the opposite Boolean value.


not
```python

not False # True

not True # False
```

## Mixing it up!
Duration: 5:00

We can combine these operators to evaluate more complex expressions.


```python

2 > 1 or 10 < 1 # True

```


## Elements of Flow Control
Duration: 5:00

Flow control statements often start with a part called the condition, and all are followed by a block of code called the clause. Before you learn about Python’s specific flow control statements, I’ll cover what a condition and a block are.

#### Condition
Something that evaluates to True or False.

#### Code Blocks
Lines of Python code can be grouped together in blocks. You can tell when a block begins and ends from the indentation of the lines of code. There are three rules for blocks.

 - Blocks begin when the indentation increases.

 - Blocks can contain other blocks.

 - Blocks end when the indentation decreases to zero or to a containing block’s indentation.

#### Example

 ```python

fish = "salmon"

if fish == "salmon":
    print("Lets make sushi!")

 ```


## If statement
 Duration: 5:00

 The most common type of flow control statement is the if statement. An if statement’s clause (that is, the block following the if statement) will execute if the statement’s condition is True. The clause is skipped if the condition is False.

 In plain English, an if statement could be read as, “If this condition is true, execute the code in the clause.” In Python, an if statement consists of the following:

The if keyword

 - A condition (that is, an expression that evaluates to True or False)

 - A colon

 - Starting on the next line, an indented block of code (called the if clause)

 ```python

fish = "salmon"

if fish == "salmon":
    print("Lets make sushi!")

 ```


## Else statement
Duration: 5:00

An if clause can optionally be followed by an else statement. The else clause is executed only when the if statement’s condition is False. In plain English, an else statement could be read as, “If this condition is true, execute this code. Or else, execute that code.” An else statement doesn’t have a condition, and in code, an else statement always consists of the following:

 - The else keyword

 - A colon

 - Starting on the next line, an indented block of code (called the else clause)


 ```python

fish = "trout"

if fish == "salmon":
    print("Lets make sushi!")
else:
    print("Mhhh, maybe we will make sushi")

 ```

## Elif statement
Duration: 5:00

While only one of the if or else clauses will execute, you may have a case where you want one of many possible clauses to execute. The elif statement is an “else if” statement that always follows an if or another elif statement. It provides another condition that is checked only if all of the previous conditions were False. In code, an elif statement always consists of the following:

- The elif keyword

- A condition (that is, an expression that evaluates to True or False)

- A colon

- Starting on the next line, an indented block of code (called the elif clause)

```python

fish = "trout"

if fish == "salmon":
    print("Lets make sushi!")
elif fish = "trout":
    print("Lets make fish stew!")
else:
    print("I dont know what we can make!")
```


## Exercise 3
Duration: 10:00

Write a program where the user is prompted to choose between three food options and print back to the user what the main ingredient is.

Example food options:

Meatballs -> beef
Sushi -> salmon
Caesar salad -> Chicken


## Loops
Duration: 5:00

You can make a block of code execute over and over again with a while statement. The code in a while clause will be executed as long as the while statement’s condition is True. In code, a while statement always consists of the following:

- The while keyword

- A condition (that is, an expression that evaluates to True or False)

- A colon

- Starting on the next line, an indented block of code (called the while clause)


Example
```python

while(True):
    print("Whoopsi!")

```

Repeater
```python

while(True):
    name = input("Please write your name: ")
    print("Hello " + name + "!")

```

## Break statement
Duration: 5:00

Break statements are shortcuts out of a loop.

```python

while(True):
    name = input("Please write your name: ")
    print("Hello " + name + "!")
    if name == "Martin":
        print("Oh, Martin!")
        break

```

## Continue statement
Duration: 5:00

Like break statements, continue statements are used inside loops. When the program execution reaches a continue statement, the program execution immediately jumps back to the start of the loop and reevaluates the loop’s condition. (This is also what happens when the execution reaches the end of the loop.)


```python

while(True):
    name = input("Please write your name: ")
    if name == "Martin":
        continue
    print("Hello " + name + "!")

```


## Exercise 4
Duration: 15:00

Write a program that continuously loops and asks the user if they want to continue. Every time the user answers yes, the program will print how many times the user has answered yes and ask the user again.

Example use:
```
Do you want to continue? yes
1
Do you want to continue? yes
2
Do you want to continue? yes
3
Do you want to continue? no

```

## For loops
Duration: 5:00

The while loop keeps looping while its condition is True (which is the reason for its name), but what if you want to execute a block of code only a certain number of times? You can do this with a for loop statement and the range() function.

In code, a for statement looks something like for i in range(5): and always includes the following:

- The for keyword

- A variable name

- The in keyword

- A call to the range() method with up to three integers passed to it

- A colon

- Starting on the next line, an indented block of code (called the for clause)

```python

for i in range(10):
    print(i)

```


## Exercise 5

Create a program that prompts the user for a number "n" and multiply it with itself "n" times.
The program will print the sum for each step in the multiplication.

#### Use a for loop to solve the exercise

Example
```
python my_multi.py
give me a number: 5
5
25
125
625
3125
```


## importing modules

All Python programs can call a basic set of functions called built-in functions, including the print(), input(), and len() functions you’ve seen before. Python also comes with a set of modules called the standard library. Each module is a Python program that contains a related group of functions that can be embedded in your programs. For example, the math module has mathematics-related functions, the random module has random number–related functions, and so on.

Before you can use the functions in a module, you must import the module with an import statement. In code, an import statement consists of the following:

 - The import keyword

 - The name of the module

 - Optionally, more module names, as long as they are separated by commas

```python
import math

math.pow(2,2) # 4.0

```


## Functions
You’re already familiar with the print(), input(), and len() functions from the previous chapters. Python provides several builtin functions like these, but you can also write your own functions. A function is like a mini-program within a program.

#### A python function

```python

def greeter(name):
    print("Hello " + str(name) + "!")

```


## Functions with return statement
When creating a function using the def statement, you can specify what the return value should be with a return statement. A return statement consists of the following:

- The return keyword

- The value or expression that the function should return


```python

def booer(name):
    return "Booo " + str(name) + "!")


result = booer("Sondre")

```


## Exercise 6

Create a function that takes a string and returns the number of A's in the string.



## None

In Python there is a value called None, which represents the absence of a value. None is the only value of the NoneType data type. (Other programming languages might call this value null, nil, or undefined.) Just like the Boolean True and False values, None must be typed with a capital N.

```python

is_none = None

```


## Keyword Arguments

keyword arguments are identified by the keyword put before them in the function call. Keyword arguments are often used for optional parameters.


```python
def booer(name):
    return "Booo " + str(name) + "!")


result = booer(name="Sondre")

```

The print() function has the optional parameters end and sep to specify what should be printed at the end of its arguments and between its arguments (separating them), respectively.

```python

print('Hello', end='')
print('World')

```

## Local and Global Scope

Parameters and variables that are assigned in a called function are said to exist in that function’s local scope. Variables that are assigned outside all functions are said to exist in the global scope. A variable that exists in a local scope is called a local variable, while a variable that exists in the global scope is called a global variable. A variable must be one or the other; it cannot be both local and global.


- Code in the global scope cannot use any local variables.

- However, a local scope can access global variables.

- Code in a function’s local scope cannot use variables in any other local scope.

- You can use the same name for different variables if they are in different scopes. That is, there can be a local variable named spam and a global variable also named spam.


#### Local variables cannot be used in global scope

```python

def my_function():
    cooking_pans = 10

print(cooking_pans) # Will throw exception!

```


## Exception Handling

Right now, getting an error, or exception, in your Python program means the entire program will crash. You don’t want this to happen in real-world programs. Instead, you want the program to detect errors, handle them, and then continue to run.

#### Exception example

```python

def zero_div():
    return 10 / 0

```

Errors can be handled with try and except statements. The code that could potentially have an error is put in a try clause. The program execution moves to the start of a following except clause if an error happens.

```python

def divide_by(number):
    try:
        return 100 / number
    except ZeroDivisionError:
        print("Error: Zero division attempted!")

```


## Exercise 7

Create a program that prompts the user for a number and a word. The the program should then print the word given by the user as many times as the number.
Additionally, make sure the program does not crash if the user inputs something else then a number. (use try/catch)

## List

A list is a value that contains multiple values in an ordered sequence. The term list value refers to the list itself (which is a value that can be stored in a variable or passed to a function like any other value), not the values inside the list value. 

#### Example

```python
my_list = [] # create a empty list

also_my_list = list() # create a empty list with the list function

cool_list = ["Some", "Data", "Items"]

```

## Getting values from a List

Say you have the list ['cat', 'bat', 'rat', 'elephant'] stored in a variable named spam. The Python code spam[0] would evaluate to 'cat', and spam[1] would evaluate to 'bat', and so on. The integer inside the square brackets that follows the list is called an index.

### Lists items can be accessed by index

```python
my_list = ["I", "am", "having", "fun"]

element = my_list[0]

print(element) # I

```

## Negative Indexes

While indexes start at 0 and go up, you can also use negative integers for the index. The integer value -1 refers to the last index in a list, the value -2 refers to the second-to-last index in a list.


```python
my_list = ["I", "am", "having", "fun"]

element = my_list[-1]

print(element) # fun

```

## Exercise 8
Create a function that takes a list and prints the first and last item in the list.

## Dictionary
Like a list, a dictionary is a collection of many values. But unlike indexes for lists, indexes for dictionaries can use many different data types, not just integers. Indexes for dictionaries are called keys, and a key with its associated value is called a key-value pair.

```python

my_dict = {"car": "volvo", "ship": "titanic"}
```