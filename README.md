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
* 

Python OOPs (Object-Oriented Programming) interview questions:

✅ Basic OOPs Concepts
What is OOPs in Python?

What are the four pillars of OOPs?

Encapsulation, Abstraction, Inheritance, Polymorphism

What is a class and an object in Python?

How is __init__ method used?

What is self in Python classes?

🔁 Inheritance & Polymorphism
What is inheritance in Python?

Types of inheritance in Python?

What is method overriding?

What is method overloading?

What is multiple inheritance?

🔒 Encapsulation & Abstraction
What is encapsulation in Python?

How do you implement abstraction?

What are private, protected, and public attributes?

🔧 Advanced OOP Concepts
What is a class method and how is it defined?

What is a static method?

What are @classmethod and @staticmethod?

What is the difference between isinstance() and issubclass()?

What is composition vs inheritance?

What are dunder/magic methods (e.g., __str__, __len__)?

What is the purpose of super()?


### Python OOPs Interview Questions and Answers

---

#### 1. What is OOPs in Python?

Object-Oriented Programming (OOP) is a programming paradigm that uses objects and classes to structure software. Python supports OOP, allowing for modular, reusable, and scalable code.

---

#### 2. What are the four pillars of OOPs?

* **Encapsulation**: Binding data and methods together and restricting access.
* **Abstraction**: Hiding complex implementation details and exposing only the necessary parts.
* **Inheritance**: Deriving new classes from existing ones.
* **Polymorphism**: Performing a single action in different ways.

---

#### 3. What is a class and an object in Python?

* **Class**: A blueprint for creating objects. It defines attributes and methods.
* **Object**: An instance of a class with actual values.

```python
class Car:
    def __init__(self, brand):
        self.brand = brand

my_car = Car("Toyota")
```

---

#### 4. How is `__init__` method used?

The `__init__` method is a constructor called when an object is instantiated. It initializes the object’s attributes.

```python
class Person:
    def __init__(self, name):
        self.name = name
```

---

#### 5. What is `self` in Python classes?

`self` represents the instance of the class. It is used to access attributes and methods within the class.

---

#### 6. What is inheritance in Python?

Inheritance allows a class (child) to inherit attributes and methods from another class (parent).

```python
class Animal:
    def speak(self):
        return "Sound"

class Dog(Animal):
    def speak(self):
        return "Bark"
```

---

#### 7. Types of inheritance in Python?

* Single
* Multiple
* Multilevel
* Hierarchical
* Hybrid

---

#### 8. What is method overriding?

Defining a method in the child class with the same name as in the parent class to change its behavior.

---

#### 9. What is method overloading?

Python does not support method overloading by default. It can be emulated using default parameters or `*args` and `**kwargs`.

---

#### 10. What is multiple inheritance?

A child class inheriting from more than one parent class.

```python
class A:
    pass
class B:
    pass
class C(A, B):
    pass
```

---

#### 11. What is encapsulation in Python?

Encapsulation is restricting access to methods and variables using access modifiers (public, protected `_`, private `__`).

---

#### 12. How do you implement abstraction?

Using abstract base classes from the `abc` module.

```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass
```

---

#### 13. What are private, protected, and public attributes?

* **Public**: Accessible from anywhere.
* **Protected**: Prefix with `_`, internal use.
* **Private**: Prefix with `__`, inaccessible directly from outside.

---

#### 14. What is a class method and how is it defined?

Class methods use `@classmethod` and take `cls` as the first parameter.

```python
class MyClass:
    count = 0

    @classmethod
    def increment(cls):
        cls.count += 1
```

---

#### 15. What is a static method?

Static methods use `@staticmethod` and do not take `self` or `cls` as arguments.

```python
class Math:
    @staticmethod
    def add(x, y):
        return x + y
```

---

#### 16. What are `@classmethod` and `@staticmethod`?

* **@classmethod**: Operates on the class.
* **@staticmethod**: Utility function with no access to class or instance.

---

#### 17. What is the difference between `isinstance()` and `issubclass()`?

* `isinstance(obj, Class)` checks if `obj` is an instance of `Class`.
* `issubclass(Sub, Super)` checks if `Sub` is a subclass of `Super`.

---

#### 18. What is composition vs inheritance?

* **Inheritance**: "is-a" relationship.
* **Composition**: "has-a" relationship; one class contains another.

---

#### 19. What are dunder/magic methods?

Special methods with double underscores like `__str__`, `__len__`, `__add__` used to define behavior of objects.

---

#### 20. What is the purpose of `super()`?

`super()` is used to call the parent class methods.

```python
class Parent:
    def show(self):
        print("Parent")

class Child(Parent):
    def show(self):
        super().show()
        print("Child")
```

