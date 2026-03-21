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
