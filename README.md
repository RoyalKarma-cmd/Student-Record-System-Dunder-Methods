# Student Record System using Dunder Methods

## Project Overview

This project demonstrates the use of Python's special methods (Dunder Methods) in an Object-Oriented Programming (OOP) environment.

The system stores student information and customizes the behavior of built-in Python functions such as:

- `print()`
- `len()`

using the special methods:

- `__init__()`
- `__str__()`
- `__len__()`

This project was developed as part of my Python and Data Science learning journey.

---

## Features

### Student Information Management

Stores:

- Student Name
- Marks
- Branch

---

## Dunder Methods Used

### `__init__()`

Initializes student objects with required information.

```python
def __init__(self, name, marks, branch):
    self.name = name
    self.marks = marks
    self.branch = branch
```

---

### `__str__()`

Provides a user-friendly representation of the object.

Example:

```python
print(student)
```

Output:

```text
Jaydeep | 95 | Extc
```

---

### `__len__()`

Returns the length of the student's name.

Example:

```python
len(student)
```

Output:

```text
7
```

---

## Code Example

```python
class Student():

    def __init__(self, name, marks, branch):
        self.name = name
        self.marks = marks
        self.branch = branch

    def __str__(self):
        return f"{self.name} | {self.marks} | {self.branch}"

    def __len__(self):
        return len(self.name)


student = Student("Jaydeep", 95, "Extc")

print(student)
print(len(student))
```

---

## Sample Output

```text
Jaydeep | 95 | Extc
7
```

---

## OOP Concepts Used

- Classes
- Objects
- Constructors
- Methods
- Dunder Methods
- Custom Object Representation

---

## Learning Outcomes

Through this project, I learned:

- How `__str__()` customizes object printing
- How `__len__()` customizes the `len()` function
- The internal working of Python special methods
- Object-Oriented Programming principles
- Creating user-friendly object representations

---

## Technologies Used

- Python
- Object-Oriented Programming (OOP)

---

## Future Improvements

- Add Grade Calculation
- Add Student ID
- Add Multiple Student Records
- Implement `__repr__()`
- Implement Operator Overloading using `__add__()`
- Build a Complete Student Management System

---

## Repository Structure

student-record-system-dunder-methods/
│
├── student_record_system.py
├── README.md
└── practice-notebook/
