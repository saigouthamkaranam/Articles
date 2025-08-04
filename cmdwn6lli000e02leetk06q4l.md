---
title: "DSA: The 8-Week Grind — Day 2"
datePublished: Mon Aug 04 2025 05:00:37 GMT+0000 (Coordinated Universal Time)
cuid: cmdwn6lli000e02leetk06q4l
slug: dsa-the-8-week-grind-day-2
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1754249183051/0857e3a1-421c-484e-a036-d31d8b80690c.png
tags: python3, software-engineering, 100daysofcode, backend-development, dsa, devjourney, codenewbies, programming-tips, learninpublic, objectorientedprogramming, pythonforbeginners, python-objectorientedprogramming-inheritance-oopinpython-pythonclasses-codereuse-programmingconcepts-pythontutorial-softwaredesign-parkinglotexample, goutham-codes

---

## **Python OOP Fundamentals — Building Code Like a Pro**

*“Functions are good. Objects are better when things get complex.”*

---

## 🟡 **Why OOP in DSA?**

Most DSA problems can be solved with functions and loops. But when problems involve **custom data structures (like Linked Lists, Trees, Graphs)** — you need **Objects & Classes**.  
OOP (Object-Oriented Programming) helps you **model real-world entities in code**.

---

## 🔹 **1\. What is Object-Oriented Programming (OOP)?**

OOP is a coding style where we structure code around **objects** — entities that hold **data (attributes)** and **behaviors (methods)**.

Think of a **"Car"**:

* Attributes: color, brand, speed
    
* Methods: accelerate(), brake(), honk()
    

---

## 🔹 **2\. Class & Object in Python**

### ➤ Define a Class:

```python
class Car:
    # Constructor
    def __init__(self, brand, color):
        self.brand = brand  # attribute
        self.color = color  # attribute
    
    # Method
    def honk(self):
        print(f"{self.brand} says Beep Beep!")
```

### ➤ Create an Object:

```python
my_car = Car("Tesla", "Red")
print(my_car.brand)  # Output: Tesla
print(my_car.color)  # Output: Red

my_car.honk()  # Output: Tesla says Beep Beep!
```

**Breakdown:**

* `class Car:` → Blueprint of an object
    
* `__init__` → Constructor that initializes object’s data
    
* `self` → Refers to the current object instance
    
* Attributes like `brand` and `color` are tied to `self`
    
* `honk()` is a method that belongs to the object
    

---

## 🔹 **3\. OOP Concepts You Need to Know (For DSA & Life)**

### ➤ Encapsulation (Data hiding with Classes)

Group related data and functions together.

```python
class BankAccount:
    def __init__(self, balance):
        self.__balance = balance  # private attribute

    def deposit(self, amount):
        self.__balance += amount

    def get_balance(self):
        return self.__balance
```

* `__balance` is private (name mangled)
    
* Access via methods like `get_balance()`
    

---

### ➤ Inheritance (Reusing Classes)

Child classes inherit properties from parent classes.

```python
class Vehicle:
    def __init__(self, brand):
        self.brand = brand

    def drive(self):
        print(f"{self.brand} is moving...")

class Car(Vehicle):
    def honk(self):
        print(f"{self.brand} says Beep!")

my_car = Car("Toyota")
my_car.drive()  # From parent class
my_car.honk()   # From child class
```

---

### ➤ Polymorphism (Same Method, Different Behaviors)

```python
class Dog:
    def speak(self):
        print("Woof")

class Cat:
    def speak(self):
        print("Meow")

def animal_sound(animal):
    animal.speak()

dog = Dog()
cat = Cat()

animal_sound(dog)  # Output: Woof
animal_sound(cat)  # Output: Meow
```

---

### ➤ Abstraction (Optional, Advanced)

Hiding internal details and showing only essential features.

```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return 3.14 * self.radius * self.radius
```

---

## 🟢 **Day 2 Takeaways:**

✅ I can now build custom Data Structures using Classes  
✅ I understand how attributes & methods shape objects  
✅ I know how to reuse and extend code using inheritance  
✅ I’m not scared of OOP jargon anymore.

---

#DSA #8WeekGrind #Day2 #PythonOOP #LearningInPublic #CodeGrind #DSAFundamentals

---