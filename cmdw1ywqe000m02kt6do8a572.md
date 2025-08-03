---
title: "DSA: The 8-Week Grind — Week-1-Day 1"
datePublished: Sun Aug 03 2025 19:06:46 GMT+0000 (Coordinated Universal Time)
cuid: cmdw1ywqe000m02kt6do8a572
slug: dsa-the-8-week-grind-week-1-day-1
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1754247971203/355888b9-8167-4e4e-8145-e73cb714ae7c.png

---

## Programming Language Fundamentals

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754181410932/68c2d88d-a982-4709-addb-f558015ed1a0.png align="center")

For my journey i am picking python because i like python.

**Python Fundamentals — Syntax, Control Structures & Functions**

---

## 🟡 **Why Start Here?**

Before diving into Data Structures & Algorithms, you need to be comfortable speaking the language.

Python is elegant, powerful, and beginner-friendly — but it’s only powerful if you know how to use it properly.

Today, I’m covering the **absolute basics that will power all my DSA problem-solving from here on**.  
Note: These are just basics to learn deeper use other free resources in youtube or refer to python documentation.

---

## 🔹 **1\. Language Syntax — Writing Python Code**

### ➤ Variables & Data Types:

```python
name = "Goutham"
age = 24
height = 5.5  # float
is_coding = True  # boolean
```

* No semicolons (`;`)
    
* No need to declare data types explicitly — Python figures it out for you.
    

### ➤ Indentation Matters:

```python
if is_coding:
    print(f"{name} is grinding DSA today!")  # 4 spaces indentation
```

⚠️ Python doesn’t use `{}` for blocks. It uses **indentation (usually 4 spaces)**.

### ➤ Comments:

```python
# This is a single-line comment

'''
This is a
multi-line comment
'''
```

---

## 🔹 **2\. Control Structures — Controlling the Flow**

### ➤ Conditional Statements:

```python
if age > 18:
    print("Adult")
elif age == 18:
    print("Just became an adult")
else:
    print("Minor")
```

* `if`, `elif`, and `else` control decision-making.
    
* Python’s syntax is clean, no parentheses needed after `if`.
    

### ➤ Loops (For & While):

### ➤ For Loop (Iterating through a list):

```python
languages = ["Python", "Java", "C++"]
for lang in languages:
    print(lang)
```

### ➤ For Loop with Range:

```python
for i in range(5):
    print(i)  # prints 0 to 4
```

### ➤ While Loop:

```python
counter = 0
while counter < 5:
    print(counter)
    counter += 1
```

### ➤ Loop Control Statements:

```python
python
CopyEdit
for i in range(10):
    if i == 5:
        continue  # skips when i == 5
    if i == 8:
        break  # stops loop when i == 8
    print(i)
```

---

## 🔹 **3\. Pseudo Code — Thinking Before Coding**

Before I code a solution, I write pseudo-code like this:

**Problem**: Find if a number is even or odd.

```plaintext
1. Input a number N
2. If N modulo 2 equals 0:
    Print "Even"
3. Else:
    Print "Odd"
```

**Python Implementation**:

```python
N = int(input("Enter a number: "))
if N % 2 == 0:
    print("Even")
else:
    print("Odd")
```

**Lesson**: **Write logic in simple steps first. Then code it.**

Pseudo-code helps you structure your thoughts before getting into syntax errors.

---

## 🔹 **4\. Functions — Breaking Problems into Blocks**

### ➤ Function Syntax:

```python
def greet(name):
    return f"Hello, {name}!"
```

### ➤ Calling Functions:

```python
python
CopyEdit
message = greet("Goutham")
print(message)  # Output: Hello, Goutham!
```

### ➤ Functions with Default Arguments:

```python
python
CopyEdit
def greet(name="Coder"):
    return f"Hello, {name}!"
```

### ➤ Functions with Multiple Parameters:

```python
python
CopyEdit
def add(a, b):
    return a + b

result = add(10, 5)
print(result)  # Output: 15
```

### ➤ Return vs Print:

* `print()` displays output.
    
* `return` sends the result back to where the function was called.
    

---

## 🟢 **Day 1 Takeaways:**

✅ Syntax clean? → Check

✅ Control structures flowing? → Check

✅ Can write logic in pseudo-code? → Check

✅ Functions modular? → Check

This is not about perfection. It’s about setting up the **coding muscle memory** for what’s coming next.

Tomorrow, we go deeper — Python OOP Concepts

---

#DSA #8WeekGrind #Day1 #PythonFundamentals #LearningInPublic #CodeGrind

---