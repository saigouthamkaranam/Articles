---
title: "DSA: The 8-Week Grind — Day 6"
seoTitle: "Master Tuples, Sets, Dictionaries & Deques in Python for DSA"
seoDescription: "Learn essential Python data structure methods for tuples, sets, dictionaries, and deques with clear explanations, code examples, and outputs. "
datePublished: Sat Aug 09 2025 02:37:42 GMT+0000 (Coordinated Universal Time)
cuid: cme3na2pn000d02jr98qf7ls4
slug: dsa-the-8-week-grind-day-6
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1754706831174/acc8a2d7-7620-465a-830f-b09f9c954668.png
tags: setup, python-tips, dictionary, dsa, tuple, day6, gouthamcodes, 8weekgrind

---

## **Other Python Data Structure Methods — Tuples, Sets, Dictionaries & Deques**

*“Strings and lists are half the game. Today, we unlock the rest.”*

---

## 🟡 Why This Day Matters

You’ve mastered strings and lists — now it’s time to learn the **other core Python data structures** that keep showing up in DSA problems.  
Today’s focus:

* **Tuples** (immutable sequences)
    
* **Sets** (unique items)
    
* **Dictionaries** (key-value mapping)
    
* **Deque** (double-ended queue)
    

---

## 🔹 **TUPLES — Immutable Sequences**

**Description**: Tuples work like lists, but they cannot be modified after creation. Perfect for fixed collections or as keys in dictionaries.

---

### ✅ Create and Access

```python
pythonCopyt = (1, 2, 3)
print(t[0])   # Output: 1
print(len(t)) # Output: 3
```

---

### ✅ `count()` — Count occurrences

**Description**: Returns how many times a value appears in the tuple.

```python
pythonCopyt = (1, 2, 2, 3)
print(t.count(2))  # Output: 2
```

---

### ✅ `index()` — Find the position of a value

**Description**: Returns the index of the first occurrence of a value.

```python
pythonCopyprint(t.index(3))  # Output: 3
```

---

## 🔹 **SETS — Unique, Unordered Collections**

**Description**: Sets store unique elements in no particular order and are very fast for membership checks.

---

### ✅ Create and Check Membership

```python
pythonCopys = {1, 2, 3}
print(2 in s)  # Output: True
```

---

### ✅ `add()` — Add a single element

**Description**: Inserts a new element into the set.

```python
pythonCopys.add(4)
print(s)  # Output: {1, 2, 3, 4}
```

---

### ✅ `update()` — Add multiple elements

**Description**: Inserts multiple values from an iterable into the set.

```python
pythonCopys.update([5, 6])
print(s)  # Output: {1, 2, 3, 4, 5, 6}
```

---

### ✅ `remove()` vs `discard()` — Remove elements

**Description**: `remove()` raises an error if element not found, `discard()` doesn’t.

```python
pythonCopys.remove(4)
s.discard(10)  # No error
print(s)       # Output: {1, 2, 3, 5, 6}
```

---

### ✅ Set Operations — `union()`, `intersection()`, `difference()`

**Description**: Combine sets, find common elements, or find unique elements.

```python
pythonCopya = {1, 2, 3}
b = {3, 4, 5}
print(a.union(b))         # Output: {1, 2, 3, 4, 5}
print(a.intersection(b))  # Output: {3}
print(a.difference(b))    # Output: {1, 2}
```

---

## 🔹 **DICTIONARIES — Key-Value Storage**

**Description**: Stores data in `{key: value}` format for quick lookups.

---

### ✅ Create and Access

```python
pythonCopyd = {"name": "Goutham", "age": 24}
print(d["name"])      # Output: Goutham
print(d.get("city"))  # Output: None
```

---

### ✅ `keys()`, `values()`, `items()` — View contents

**Description**: Retrieve all keys, values, or both.

```python
pythonCopyprint(list(d.keys()))   # Output: ['name', 'age']
print(list(d.values())) # Output: ['Goutham', 24]
print(list(d.items()))  # Output: [('name', 'Goutham'), ('age', 24)]
```

---

### ✅ `update()` — Merge dictionaries

**Description**: Adds or updates key-value pairs from another dictionary.

```python
pythonCopyd.update({"city": "Hyderabad"})
print(d)  # Output: {'name': 'Goutham', 'age': 24, 'city': 'Hyderabad'}
```

---

### ✅ `pop()` — Remove a key by name

**Description**: Deletes the specified key and returns its value.

```python
pythonCopyd.pop("age")
print(d)  # Output: {'name': 'Goutham', 'city': 'Hyderabad'}
```

---

### ✅ `popitem()` — Remove last inserted pair

**Description**: Removes and returns the last key-value pair.

```python
pythonCopyd.popitem()
print(d)  # Output: {'name': 'Goutham'}
```

---

## 🔹 **DEQUE — Double-Ended Queue**

**Description**: From `collections`, lets you add/remove from both ends in O(1) time.

---

### ✅ Create a Deque

```python
pythonCopyfrom collections import deque
dq = deque([1, 2, 3])
print(dq)  # Output: deque([1, 2, 3])
```

---

### ✅ `append()` and `appendleft()` — Add to ends

**Description**: Add elements to right or left end.

```python
pythonCopydq.append(4)
dq.appendleft(0)
print(dq)  # Output: deque([0, 1, 2, 3, 4])
```

---

### ✅ `pop()` and `popleft()` — Remove from ends

**Description**: Remove and return elements from right or left end.

```python
pythonCopydq.pop()
dq.popleft()
print(dq)  # Output: deque([1, 2, 3])
```

---

### ✅ `extend()` and `extendleft()` — Add multiple elements

**Description**: Add elements from iterable to right or left end.

```python
pythonCopydq.extend([5, 6])
dq.extendleft([-1, -2])
print(dq)  # Output: deque([-2, -1, 1, 2, 3, 5, 6])
```

---

## 🟢 **Day 6 Takeaways**

✅ Tuples: Immutable, safe for fixed data  
✅ Sets: Unique, fast membership checks  
✅ Dictionaries: Key-value data mapping  
✅ Deque: Efficient double-ended operations

---