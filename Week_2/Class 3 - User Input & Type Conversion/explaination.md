# ⌨️ Class 3: User Input & Type Conversion

Welcome to **Class 3!** 🚀

Up until now, our programs have been static. In this session, we’ll learn how to make programs interactive by accepting **User Input**. We will also explore **Type Conversion** to ensure our data behaves the way we want it to (especially when doing math!).

---

## 📥 What is User Input?
Programs become truly useful when they interact with users. User input allows your program to:
* Ask questions
* Accept data
* Respond dynamically based on what the user types

In Python, we use the `input()` function to get data from the user.

### Example:
```python
name = input("Enter your name: ")
print("Hello", name)
```

**What’s happening here?**
1. The program waits for the user to type something and press **Enter**.
2. Whatever the user types is stored in the variable `name`.

---

## ⚠️ How `input()` Works
It is crucial to understand that `input()` **always returns text (string)**.

Even if you type a number (like `25` or `100`), Python treats it as a text string, not a number. Python does **NOT** automatically convert data types for you.

### Checking the Data Type:
```python
age = input("Enter your age: ")
print(type(age))
```
**Output:**
```text
<class 'str'>
```
> **✔ Important:** You cannot do math on strings immediately!

---

## 🧮 Why Type Conversion is Needed
Mathematical operations require numeric data. If you try to add two numbers taken directly from `input()`, Python will join them together like text (**concatenation**) instead of adding them mathematically.

### The Wrong Way ❌
```python
a = input("Enter number: ")
b = input("Enter number: ")

print(a + b)
```
**Result:**
If user enters `2` and `3`:
* **Output:** `"23"` (This is string joining, not addition!)

---

## 🔄 Type Conversion Functions
To fix the issue above, Python provides built-in functions to convert data types. This is often called "**casting**."

* `int()` → Converts to **Integer** (whole numbers)
* `float()` → Converts to **Decimal** numbers
* `str()` → Converts to **String** (text)

### The Correct Way ✔
```python
# Convert input immediately to integer
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print(a + b)
```
**Result:**
Now, if the user enters `2` and `3`, the output will be `5`.

---

## 💸 Using `float()` for Decimal Values
You should use `float()` when dealing with numbers that might have decimals, such as **money, averages, or percentages**.

### Example: Calculating a Bill
```python
price = float(input("Enter price: "))
tax = float(input("Enter tax: "))

total = price + tax
print("Total amount:", total)
```

---

## 🚫 Common Input Mistakes
When working with inputs, watch out for these common errors:

* ❌ **Forgetting type conversion** (Trying to do math on strings).
* ❌ **Using the wrong data type** (e.g., trying to convert "hello" to an integer).
* ❌ **Assuming input is already a number.**

### Bad Code ❌
```python
age = input("Enter age: ")
print(age + 5)   # Error: cannot add integer to string
```

### Good Code ✔
```python
age = int(input("Enter age: "))
print(age + 5)   # Success!
```

---

## 📝 Practice Tasks
- [ ] **Greeting App:** Ask the user for their name and favorite color, then print a sentence using both.
- [ ] **Age Calculator:** Ask the user for their birth year, subtract it from the current year, and print their age.
- [ ] **Simple Adder:** Ask for two numbers (integers), add them, and print the result.
- [ ] **Grocery Calculator:** Ask for the price of an item (float) and the quantity (int), then calculate the total cost.

---

### 🧠 Why This Works
* **Interactive Learning:** You aren't just reading code; you are talking to the program.
* **Real-World logic:** Almost every app needs user input (logins, forms, search bars).
* **Error Handling:** Teaches you to be careful about data types early on.