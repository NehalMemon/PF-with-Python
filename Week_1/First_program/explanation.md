# 🧠 Class 2: Comments, Escape Sequences, Variables & Data Types

Welcome back! 👋  
In this class, we’ll learn some of the most important building blocks of Python — how to write comments, use escape sequences, store data using variables, and understand basic data types.

---

## 💬 Comments in Python

Comments are lines in your code that Python ignores when running.  
They’re meant for humans, not the computer — to explain what your code does.

### 📝 Why Use Comments?

- To describe your code for yourself and others  
- To make debugging easier  
- To temporarily disable lines of code  

---

## 🧩 Types of Comments

### 1️⃣ Single-line Comment
```python
# This is a single-line comment
print("Hello, World!")  # This prints a message
```
### 2️⃣ Multi-line Comment
```python
"""
This is a multi-line comment.
It can be used to describe larger sections of code.
"""
print("Welcome to Python!")
```
✅ Tip: Always comment your code to make it more readable!

## 🔠 Escape Sequences

Escape sequences let you insert special characters inside strings — like new lines or tabs.

### 🧩 Common Escape Sequences

| Escape | Description | Example |
|:-------|:-------------|:---------|
| `\n` | New line | `"Hello\nWorld"` |
| `\t` | Tab space | `"Hello\tWorld"` |
| `\\` | Backslash | `"This is a backslash: \\"` |
| `\"` | Double quote | `"He said, \"Hi!\""` |
| `\'` | Single quote | `'It\'s a sunny day'` |

### 🧠 Example
```python
print("Hello\nWorld")       # Prints on two lines
print("Name:\tNehal")       # Adds a tab between text
print("He said, \"Welcome!\"")
```
### Output:
```python
Hello
World
Name:    Nehal
He said, "Welcome!"
```
# 📦 Variables

Variables are like containers that store data in memory.
They help your program remember information while it runs.

## ✨ Creating Variables
```python
name = "Ahmed"
age = 21
language = "Python"

print(name)
print(age)
print(language)
```
### Output:
```python
Ahmed
21
Python
```

## 🧠 Rules for Variable Names

- Must start with a letter or underscore (_)

- Can contain letters, numbers, or underscores

- Case-sensitive (Name and name are different)

- Avoid using Python keywords like print, if, for, etc.

✅ Good variable names: user_name, total_score, temperature
❌ Bad variable names: 1name, print, a b

# 🧮 Data Types in Python

Data types tell Python what kind of value a variable holds.

###  Basic Data Types

| Type | Example | Description |
|:------|:----------|:-------------|
| `int` | `10`, `-5` | Whole numbers |
| `float` | `3.14`, `-2.5` | Decimal numbers |
| `str` | `"Hello"`, `'World'` | Text (string) |
| `bool` | `True`, `False` | Logical values |

# 🧠 Example
```python
name = "Nehal"
age = 21
height = 5.9
is_student = True

print(type(name))
print(type(age))
print(type(height))
print(type(is_student))
```
### Output:
```python
<class 'str'>
<class 'int'>
<class 'float'>
<class 'bool'>
```
## 🧩 Type Casting (Converting Data Types)

You can convert one data type into another using type casting.
```python
age = "21"
age = int(age)        # Convert string to integer
print(age + 5)
```
Output:
```python
26
```

# 🔍 Practice Tasks

✅ 1. Write a program that stores your name, age, and favorite color in variables and prints them.

✅ 2. Use escape sequences to display this pattern:
