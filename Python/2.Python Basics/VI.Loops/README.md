# Loops

🔹 for Loop
Used to iterate (loop) over a sequence like a list, string, or range.

✅ Basic syntax:
```
for variable in sequence:
    # code block
```
Example with range():
```
for i in range(5):
    print(i)  # prints 0 to 4
```
🔹 range(start, stop, step) in Loops
range(5) → 0 to 4

range(1, 6) → 1 to 5

range(1, 10, 2) → 1, 3, 5, 7, 9

```
for i in range(1, 6):
    print("Hi", i)
```
🔹 while Loop
Repeats while a condition is True.

✅ Syntax:
```
while condition:
    # code block
```
Example:
```
x = 1
while x <= 5:
    print(x)
    x += 1
```
🔹 Loop Control Statements
🔸 break: stop the loop early
```
for i in range(10):
    if i == 5:
        break
    print(i)  # stops at 4
```
🔸 continue: skip the current loop iteration
```
for i in range(5):
    if i == 2:
        continue
    print(i)  # skips 2
```
🔸 pass: placeholder that does nothing
```
for i in range(3):
    pass  # do nothing
```
🔹 else with Loops
Runs if loop was not stopped by break.
```
for i in range(5):
    print(i)
else:
    print("Loop finished!")  # runs only if no break
```
## 3.Examples Only Based on Loops
✅ Simple Loop Examples
```
# Print 1 to 5 using for
for i in range(1, 6):
    print(i)

# Print numbers using while
x = 3
while x > 0:
    print(x)
    x -= 1

# Use break
for i in range(10):
    if i == 4:
        break
    print(i)  # 0 to 3

# Use continue
for i in range(5):
    if i == 2:
        continue
    print(i)  # skips 2
```
# Tricky Loop Examples
```
# Tricky 1: Empty range
for i in range(5, 1):
    print(i)  # Does nothing

# Tricky 2: Step backwards
for i in range(5, 0, -1):
    print(i)  # 5 4 3 2 1

# Tricky 3: Infinite while (be careful!)
x = 1
while True:
    print(x)
    if x == 3:
        break
    x += 1

# Tricky 4: continue in while loop
x = 0
while x < 4:
    x += 1
    if x == 2:
        continue
    print(x)  # skips 2

# Tricky 5: else with break
for i in range(5):
    if i == 3:
        break
    print(i)
else:
    print("Done")  # Won't run because of break
```
# 4. ✅ Tips to Master Python Loops

| Tip No. | Tip                                                                                  |
| ------- | ------------------------------------------------------------------------------------ |
| 1️⃣     | Use `for i in range(n)` when you know how many times to repeat.                      |
| 2️⃣     | Use `while` when looping until a condition changes.                                  |
| 3️⃣     | `break` exits the loop completely.                                                   |
| 4️⃣     | `continue` skips current iteration only.                                             |
| 5️⃣     | Be careful of **infinite loops**—make sure `while` loops have an exit condition.     |
| 6️⃣     | `range(start, stop, step)` can go up or down—step can be negative.                   |
| 7️⃣     | Use `else` with loops only if you want to do something **after loop ends normally**. |

