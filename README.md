### 👌 Basic-Level Questions

#### 1. Is Python a compiled or interpreted language?

Python is an **interpreted language**. It is compiled to bytecode (`.pyc`) and then executed by the Python Virtual Machine (PVM).

#### 2. How can you concatenate two lists in Python?

```python
list1 = [1, 2]
list2 = [3, 4]
result = list1 + list2  # [1, 2, 3, 4]
```

#### 3. What is the difference between for loop and while loop in Python?

* `for`: Iterates over a sequence.
* `while`: Loops while a condition is true.

#### 4. How do you floor a number in Python?

```python
import math
math.floor(4.7)  # Output: 4
```

#### 5. What is the difference between `is` and `==` in Python?

* `is`: Compares memory locations.
* `==`: Compares values.

#### 6. What are the common built-in data types in Python?

* Numeric: `int`, `float`, `complex`
* Sequence: `list`, `tuple`, `range`
* Text: `str`
* Set: `set`, `frozenset`
* Mapping: `dict`
* Boolean: `bool`
* Binary: `bytes`, `bytearray`, `memoryview`
* None: `NoneType`

#### 7. What is `__init__` in Python?

A special constructor method to initialize object properties.

#### 8. What is the difference between Python arrays and lists?

| Feature     | list        | array (`array` module) |
| ----------- | ----------- | ---------------------- |
| Types       | Mixed types | Single data type only  |
| Flexibility | High        | Optimized for numbers  |

#### 9. What is PYTHONPATH?

An environment variable that specifies where Python looks for modules.

#### 10. What are list comprehensions, and how are they useful?

A concise way to create lists:

```python
[x*x for x in range(5)]  # [0, 1, 4, 9, 16]
```

---

### 🔀 Intermediate-Level Questions

#### 1. What is the difference between a list and a tuple in Python?

* `list`: Mutable, uses `[]`
* `tuple`: Immutable, uses `()`

#### 2. How do you convert a list into a tuple?

```python
tuple([1, 2, 3])
```

#### 3. How would you convert a list into an array?

```python
from array import array
array('i', [1, 2, 3])
```

Or using NumPy:

```python
import numpy as np
np.array([1, 2, 3])
```

#### 4. How is memory managed in Python?

* Reference counting
* Garbage collection
* Memory pools

#### 5. What are the key features of Python?

* Simple syntax
* Interpreted
* Dynamically typed
* Cross-platform
* Extensive libraries
* OOP and functional support

#### 6. What are keywords in Python?

Reserved words (e.g., `if`, `class`, `return`).

```python
import keyword
print(keyword.kwlist)
```

#### 7. What are literals in Python and explain different types?

* Numeric: `123`
* String: `'abc'`
* Boolean: `True`, `False`
* None: `None`
* Collections: `[1]`, `(1,)`, `{1}`, `{'a':1}`

#### 8. How can you concatenate two tuples?

```python
(1, 2) + (3, 4)  # (1, 2, 3, 4)
```

#### 9. What is the difference between classes and instances?

* Class: Blueprint
* Instance: Object created from a class

#### 10. What are ternary operators in Python?

```python
x = 10
result = 'Even' if x % 2 == 0 else 'Odd'
```

---

### 🧠 Advanced-Level Questions

#### 1. What is the difference between shallow copy and deep copy?

```python
import copy
shallow = copy.copy(obj)
deep = copy.deepcopy(obj)
```

#### 2. How does multi-threading work in Python?

* Via `threading` module
* Limited by GIL (only one thread runs bytecode)
* Best for I/O-bound tasks

#### 3. What are decorators in Python?

Functions that modify other functions:

```python
@decorator
def func(): pass
```

#### 4. When are `*args` and `**kwargs` used?

* `*args`: Variable positional arguments
* `**kwargs`: Variable keyword arguments

#### 5. What is the difference between `help()` and `dir()` functions?

* `help(obj)`: Shows documentation
* `dir(obj)`: Lists attributes/methods

#### 6. How are arguments passed in Python: by value or by reference?

* Python uses **call by object reference**
* Mutable objects can be changed; immutable can't

#### 7. What is monkey patching in Python?

Modifying classes/modules at runtime.

```python
import math
math.sqrt = lambda x: "patched!"
```

#### 8. What is the difference between `is` and `==`?

* `is`: Same memory
* `==`: Same value

#### 9. What is the purpose of the `groupby()` function in Pandas?

Groups data and applies aggregate functions:

```python
df.groupby('col')['val'].sum()
```

#### 10. What is the difference between `.loc` and `.iloc` in Pandas?

* `.loc`: Label-based
* `.iloc`: Index-based

#### 11. Why is Python considered an interpreted language?

* Compiled to bytecode (`.pyc`), then interpreted by PVM
* No machine code compilation
* Easier debugging and portability
