## 🔹 1. What is a Variable in Python?

A variable is a name that refers to a value stored in memory. It acts like a container where you store data (numbers, text, etc.) for later use.

```
name = "Gokulnath"
age = 24
```
🔹 2. Rules for Naming Variables

| Rule                                         | Example           | Valid? |
| -------------------------------------------- | ----------------- | ------ |
| Can contain letters, digits, and underscores | `user_name1`      | ✅ Yes  |
| Cannot start with a number                   | `1name = "Gokul"` | ❌ No   |
| Cannot use Python keywords                   | `class = 10`      | ❌ No   |
| Case-sensitive                               | `name` ≠ `Name`   | ✅ Yes  |

🔹 3. Variable Types (Dynamically Typed Language)
Python automatically detects variable type.

```
name = "Gokul"      # str
age = 25            # int
height = 5.9        # float
is_active = True    # bool
```
You can check type using:
```
print(type(name))  # Output: <class 'str'>
```

🔹 4. Multiple Variable Assignment
```
a, b, c = 1, 2, 3
x = y = z = 100
```

🔹 5. Variable Reassignment
```
age = 25
age = "Twenty-five"  # Now it's a string
```
🔹 6. Constants (Not real constants but uppercase naming used conventionally)
```
PI = 3.14
MAX_USERS = 100
```
🔹 7. Memory Reference / ID
```
x = 10
print(id(x))  # Shows memory location
```
🔹 8. Input from User and Store in Variable
```
name = input("Enter your name: ")
print("Hi", name)
```
🔹 9. Variable Scope
| Scope  | Description                       |
| ------ | --------------------------------- |
| Global | Accessible anywhere in the script |
| Local  | Accessible only within a function |

```
x = "global"

def show():
    x = "local"
    print(x)  # local

show()
print(x)      # global
```
🔹 10. Type Casting
Convert one type to another.
```
a = "100"
b = int(a)  # Converts string to integer
```

## 🛠️ PRACTICAL REAL-TIME EXAMPLES — Python Variables Only

✅ Example : User Profile

```
name = "Gokul"
age = 24
city = "Coimbatore"

print("Name:", name)
print("Age:", age)
print("City:", city)

```

⚡ Example 1: Value Overwriting Confusion

```
user = "Arun"
user = "Divya"
user = "Muthu"

print("Final user:", user)
```

🧠 Output: Muthu
🎯 Reason: Variables always store the latest assigned value, older ones are lost.

⚡ Example 2: Variable Reference Copy
```
a = 500
b = a
a = 300

print("a:", a)
print("b:", b)
```
🎯 Reason: b got the value before a changed, not linked forever.

⚡ Example 3: Swapping Without Temp Variable
```
x = 10
y = 20

x, y = y, x

print("x:", x)
print("y:", y)
```
🎯 Python supports tuple unpacking for clean swapping.

⚡ Example 4: Type Change Midway
```
var = 123         # int
var = "123"       # now string
var = [123]       # now list

print("var:", var)
print("Type:", type(var))
```
🎯 Python allows dynamic typing — variable type changes any time.

⚡ Example 5: Memory Sharing for Small Integers
```
a = 100
b = 100

print(id(a) == id(b))  # True for small integers (−5 to 256)
```
🎯 Python internally optimizes by pointing to the same memory for small integers.

⚡ Example 6: String Multiplication
```
name = "🔥"
repeat = 5

banner = name * repeat
print("Banner:", banner)
```
🎯 You can multiply strings with integers in Python!

⚡ Example 7: Variable Chaining
```
a = b = c = "Python"

print(a, b, c)
```
🎯 All variables point to the same string in memory.

⚡ Example 8: Using id() to Understand Memory
```
x = 256
y = 256

print(id(x), id(y))  # Same

x = 300
y = 300

print(id(x), id(y))  # Might differ
```
🎯 Python caches small integers between -5 to 256.

⚡ Example 9: Boolean as Integer
```
a = True
b = False

print(a + 5)    # 1 + 5 = 6
print(b + 10)   # 0 + 10 = 10
```
🎯 In Python, True = 1, False = 0 (they are subclasses of int!)

⚡ Example 10: Shadowing Built-in Names
```
list = "Not a list"
print(list)

# Real list can't be used now
# my_list = list([1,2,3])  # ❌ Error if uncommented
```
🎯 Avoid using built-in names like list, str, int as variables — you shadow Python’s core functions.
