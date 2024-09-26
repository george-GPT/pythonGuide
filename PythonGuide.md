### Python: Efficent Learning Guide
## Common Syntax
```python
import module
var_x = 10
int_x = 5
float_y = 3.14
string = "George"
(f"Hello, {string}") 
bool_test = False
def function_name(param1, param2) 
Ordered/Changeable: list = ['apple', 'banana', 'cherry']
Ordered/Fixed: tuple = ('apple', 'banana', 'cherry')
Unordered/Key Value Pairs: dict = {'name': 'apple', 'type': 'fruit'}
print()
input() takes user input
len() Returns length 
int(), str(), float() Convert between data types
range() Generates a sequence of numbers
for item in iterable(): 
for key, value in person.items():
while condition:
Control Flow: if, elif, else, for, while, break, continue, return
Exception Handling: try, except, finally, raise, assert
Logical Operators: and, or, not, is, in
Variable/Scope Modifiers: global, nonlocal, pass, del
Data Types & Constants: True, False, None
Imports: import, from, as
Other: with, async, await
random.randint(1, 10)
random.choice(['apple', 'banana', 'cherry'])
random.shuffle([1, 2, 3, 4, 5])
file = open('filename.txt', 'r')
content = file.read()
```

## Control Flow (if, elif, else, while)
```python
number = float(input("Enter a number: "))
if number > 0:
    print("Positive")
elif number < 0:
    print("Negative")
else:
    print("Zero")


count = 1
while count <= 3:
    print(count)
    count += 1  # Increment count

while True:
    item = input("Enter an item to add to the list (type 'done' to finish): ")
    if item.lower() == 'done':
        print("Final list:", collected_items)
        break
    collected_items.append(item)
    print(f"Current list: {collected_items}")

# Define a dict
person = {'name': 'Alice', 'age': 25}
# Get user input for key
key = input("Enter the key you want to access (name/age): ")
# Check and print the value
if key in person:
    print(f"{key.capitalize()}: {person[key]}")
elif key == "address":
    print("Address key exists but has no value.")
else:
    print("Key not found.")
```

## Control Flow (Looping with for in)
```python
Looping over list
fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
    print(fruit)
    
Looping over list (range)
fruits = ['apple', 'banana', 'cherry']
for i in range(5):
    print(i)
    
looping over list (index)
for i in range(len(fruits)):
    print(i, fruits[i])
    
Looping over a dict
person = {'name': 'Alice', 'age': 25}
for key, value in person.items():
    print(key, value)

Loop (continue, break) 
for i in range(5):
    if i == 2:
        continue  # Skip when i is 2
    if i == 4:
        break  # Stop the loop when i is 4
    print(i)
