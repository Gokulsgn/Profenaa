## 1.  What are Python Conditions?

Conditions let your program make decisions.

Python uses:

if

elif (else if)

else
to run different blocks of code based on whether a condition is True or False.
2. 📚 All Concepts of Python Conditions
🔹 Basic Structure
```
if condition:
    # code runs if condition is True
elif another_condition:
    # runs if first was False, and this is True
else:
    # runs if none above are True
```
✅ The condition is usually a comparison like ==, >, <, etc.
🔹 Comparison inside if
You can use:

== (equal)

!= (not equal)

>, <, >=, <=
```
x = 5
if x == 5:
    print("It is five")
```
🔹 elif (else if)
Used to check multiple conditions.
```
x = 10
if x < 5:
    print("Small")
elif x == 10:
    print("Ten")  # this runs
else:
    print("Other")
```
🔹 else block
Used if all above conditions are False.
```
x = 7
if x > 10:
    print("Big")
else:
    print("Not big")  # this runs
```
🔹 Logical Operators in Conditions
You can combine conditions with:

and – True if both are True

or – True if at least one is True

not – Reverses the condition
```
age = 20
if age > 18 and age < 25:
    print("Young adult")
```
🔹 Nested Conditions
An if inside another if.
```
x = 10
if x > 5:
    if x < 15:
        print("Between 5 and 15")  # This runs
```
🔹 Truthy & Falsy in Conditions
Any value can be used in if. Some are automatically treated as:

False: 0, "", [], {}, None, False

True: anything else
```
name = ""
if name:
    print("You entered something")
else:
    print("Empty input")  # This runs
```
3. 🔍 Examples Only Based on Conditions
✅ Simple Condition Examples
```
x = 5
if x > 0:
    print("Positive")

x = 3
if x % 2 == 0:
    print("Even")
else:
    print("Odd")

x = 100
if x > 90:
    print("Excellent")
elif x > 75:
    print("Good")
else:
    print("Try again")
```
Tricky Condition Examples
```
# Tricky 1: Chained condition
x = 8
if 5 < x < 10:
    print("In range")  # Runs

# Tricky 2: Multiple elif but one match
x = 7
if x < 5:
    print("Small")
elif x < 10:
    print("Medium")  # Runs
elif x < 20:
    print("Large")

# Tricky 3: Use of not
value = ""
if not value:
    print("Empty!")  # Runs

# Tricky 4: Nested condition
x = 4
y = 2
if x > 3:
    if y < 3:
        print("Nested True")  # Runs

# Tricky 5: Boolean shortcut
x = 0
if x:
    print("This won't run")
else:
    print("Zero is False")  # Runs
```
## 4. ✅ Tips to Master Python Conditions
| Tip No. | Tip                                                                         |
| ------- | --------------------------------------------------------------------------- |
| 1️⃣     | Indentation matters! Code inside `if`, `else`, etc. must be indented.       |
| 2️⃣     | Use `elif` when checking multiple exclusive options.                        |
| 3️⃣     | `and`, `or`, and `not` make conditions powerful—learn to combine them well. |
| 4️⃣     | Any non-zero, non-empty value is **True** in conditions.                    |
| 5️⃣     | Always test all branches: `if`, `elif`, `else` to be sure.                  |
| 6️⃣     | You can nest conditions, but don't overdo—it can get messy.                 |
| 7️⃣     | Prefer `if ... elif ... else` instead of many `if` statements.              |


