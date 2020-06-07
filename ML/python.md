---
layout: default
---

# Python Crash Course

## Representing Variables, Strings and Integers

Variables are used to store values. A string is a series of characters, surrounded by single or double quotes.

### Variables
```
msg = "Hello world!" 
print(msg)
```
### Strings
```
print("Hello world!")
```

### Integers

```
msg = 1   #Integer
print(msg)
```

## Concatenation (combining strings)

```
first_name = 'albert'
last_name = 'einstein'
full_name = first_name + ' ' + last_name
print(full_name)
```
## List

A list stores a series of items in a particular order. You access items using an index, or within a loop.

### Make a list
```
bikes = ['trek', 'redline', 'giant']
```
### Get the first item in a list

```
first_bike = bikes[0]  
```
### Get the last item in a list

```
last_bike = bikes[-1]                      
```

### Looping through a list

```
for bike in bikes:                         
 print(bike)
```

### Adding items to a list

```
bikes = []                                 
bikes.append('trek')
bikes.append('redline')
bikes.append('giant')
```

### Making numerical lists using range()

```
squares = []                               
for x in range(1, 11):
 squares.append(x**2)
 ```

### List comprehensions

```
squares = [x**2 for x in range(1, 11)]
```

### Slicing a list
```
finishers = ['sam', 'bob', 'ada', 'bea']
first_two = finishers[:2]
```

### Copying a list
```
copy_of_bikes = bikes[:]
```

## Tuples

Tuples are similar to lists, but the items in a tuple can't be modified.

### Making a tuple

```
dimensions = (1920, 1080)
```

## Operators

### if Statements
If statements are used to test for particular conditions and respond appropriately.

##### Conditional tests

```
equals x == 42
not equal x != 42
greater than x > 42
 or equal to x >= 42
less than x < 42
 or equal to x <= 42
 ```
 
##### Conditional test with lists

```
'trek' in bikes
'surly' not in bikes
```

##### Assigning boolean (TRUE or FALSE) values

```
game_active = True
can_edit = False
```

#### if Statement Sample

```
if age >= 18:
 print("You can vote!")
 ```
 
#### If-elif-else statements

```
if age < 4:
 ticket_price = 0
elif age < 18:
 ticket_price = 10
else:
 ticket_price = 15
 ```
 #### While Loops
 
A while loop repeats a block of code as long as a certain condition is true.

##### A simple while loop
```
current_value = 1

while current_value <= 5:
 print(current_value)
 current_value += 1
```

## Classes

A class defines the behavior of an object and the kind of information an object can store. The information in a class is stored in attributes, and functions that belong to a class are called methods. A child class inherits the attributes and methods from its parent class.

### Creating a dog class

```
class Dog():
 """Represent a dog."""
 def __init__(self, name):
 """Initialize dog object."""
 self.name = name
 def sit(self):
 """Simulate sitting."""
 print(self.name + " is sitting.")
my_dog = Dog('Peso')
print(my_dog.name + " is a great dog!")
my_dog.sit()
```

### Inheritance

```
class SARDog(Dog):
 """Represent a search dog."""
 def __init__(self, name):
 """Initialize the sardog."""
 super().__init__(name)
 def search(self):
 """Simulate searching."""
 print(self.name + " is searching.")
my_dog = SARDog('Willie')
print(my_dog.name + " is a search dog.")
my_dog.sit()
my_dog.search()
```
