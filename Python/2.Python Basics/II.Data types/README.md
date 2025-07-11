# 1. What are Data Types?

In Python, data types define the type of value a variable holds — whether it's a number, text, list, etc. Python is dynamically typed, so it detects data types automatically.

# 2. Built-in Data Types in Python
| Category      | Data Types                         |
| ------------- | ---------------------------------- |
| Text Type     | `str`                              |
| Numeric Type  | `int`, `float`, `complex`          |
| Sequence Type | `list`, `tuple`, `range`           |
| Mapping Type  | `dict`                             |
| Set Type      | `set`, `frozenset`                 |
| Boolean Type  | `bool`                             |
| Binary Type   | `bytes`, `bytearray`, `memoryview` |
| None Type     | `NoneType`                         |

# 3. Commonly Used Data Types with Examples

✅ String (str)
```
name = "Gokulnath"
```
A sequence of characters.

Enclosed in ' ' or " ".

✅ Integer (int)
```
age = 25
```
Whole numbers.

✅ Float (float)
```
height = 5.9
```
Decimal numbers.

✅ Boolean (bool)
```
is_active = True
```
Only True or False.

✅ List (list)
```
skills = ["Python", "SQL", "Power BI"]
```
Mutable, ordered collection.

Supports duplicates.

✅ Tuple (tuple)
```
marks = (80, 90, 85)
```
Immutable, ordered collection.

✅ Dictionary (dict)
```
student = {"name": "Gokul", "age": 25, "course": "AI"}
```
Key-value pairs.

Unordered (as of Python 3.6+, insertion-ordered).

✅ Set (set)
```
unique_skills = {"Python", "SQL", "Power BI"}
```
Unordered, unique elements.

✅ None (NoneType)
```
value = None
```
Used to define null or empty value.

# 4. Type Checking and Casting
```
print(type(name))  # <class 'str'>
print(int("100"))  # 100
```

