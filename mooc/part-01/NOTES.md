# Python Programming MOOC 2026 - Part 1 (Lecture Notes)

> **Introduction to Programming** | [Programming '26 MOOC](programming-26.mooc.fi/part-1).

---
## Table of Contents

1. [Getting Started](#1-getting-started)
2. [Information from the User](#2-information-from-the-user)
3. [More about Variables](#3-more-about-variables)
4. [Arithmetic Operations](#4-arthmetic-operations)
5. [Conditional Statements](#5-conditional-statements)
6. [Quick Reference Cheatsheet](#quick-reference-cheatsheet)

---

## 1. Getting Started

A program is a sequence of commands executed one by one, **from top to bottom**. Programming is the process of writing those programs that instruct a computer to perform specific tasks or tell a computer how to solve problems and carry out instructions.

- Programs executes line by line **(from top to bottom)**
- The computer follows exact instructions.

### Output with the `print()` Command

```python
print("Hello, world!")
```

- This is used to display output to the screen
- Texts (strings) must be inside quotes, **single ' '** or **double " "**

### Multiple Commands

```python
print("Welcome to Introduction to Programming!")
print("First we will practice using the print command.")
print("This program prints three lines of text on the screen.")
```

- This is a program of multiple commands.
- This commands are executed sequentially, from first to last.

### Arithmetic in `print`

```python
print(2+5) # -> 7
print(3+3) # -> 9
print(2 + 2 * 10) # -> 22
```

- Arithmetics can be done inside a `print` command.
- Running it would perform the operation and print out the result.

Wrapping a calculation in quotes prints it as **literal text** instead:

```python
print(2 + 2 * 10) # -> 22
print("2 + 2 * 10") # -> 2 + 2 * 10
```

### Comments

Any line beginning with the pound or hash sign `#` is a comment. Python ignores it completely, which means any command following the `#` symbol will not affect the program in any way.

```python
# There are 365 days in a year and 24 hours in each day
print(365 * 24) # outputs 8760
```

> Good comments explain **why** or **how** a command, program, or code works or does something.

---

## 2. Information From The User

`Input` refers to any information a user gives to the program. The Python command `input()` reads in a line of input typed in by the user. It may also be used to prompt the user for a specific input, and used to display a message to the user.

> `input()` pauses the program, shows a prompt, and returns whatever the user types in as a string.

```python
name = input("What is your name? ")
print("Hi there, " + name)  # outputs "Hi there, David"
```

### Variables

A variable is a named storage location in memory. It is also a location for storing a value, such as a string or a number. This value can be used later, and it can also be changed.

#### Naming Rules:

- Must start with a letter or underscore **_**
- Can contain letters, digits, and underscores
- Case-sensitive: name, Name, and NAME are three different variables
- Conventional practice: use lowercase_with_underscores

> A variable stores only its most recent value. Previous values are overwritten and lost.

### String Concatenation

Concatenation is how strings are combined using the `+` opeerator. Strings and variables can be combined freely.

```python
name = input("What is your name? ")
print("Hi " + name + "! Nice to meet you.")

""" Output
Whats is your name? David
Hi David! Nice to meet you. """
```

### Multiple Inputs

A program can ask for more than one input. Notice how below each `input` command stores the received value in a different variable.

```python
name = input("What is your name? ")
email = input("What is your email address? ")
nickname = input("What is your nickname? ")

print("Let's make sure we got this right")
print("Your name: " + name)
print("Your email address: " + email)
print("Your nickname: " + nickname)
```

### Overwriting a Variable

If the same variable is used to store more than one input, each new value will replace the previous one. Same way as if the same variable is used to store two inputs in succession, there is no way to access the first input value after it has been replaced by the second.

```python
address = input("Current address: ")
print("You live at " + address)

address = input("New address: ")
print("Your new address is " + address)
```

---

## 3. More About Variables
