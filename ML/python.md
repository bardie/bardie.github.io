---
layout: default
---

# Python Crash Course

## Representing Variables, Strings and Integers

Variables are used to store values. A string is a series of characters, surrounded by single or double quotes.

### Variables
```
msg = "Hello world!"   #Variable
print(msg)
```
### Strings
```
print("Hello world!")  #String
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

Make a list
```
bikes = ['trek', 'redline', 'giant']
first_bike = bikes[0]                      #Get the first item in a list
last_bike = bikes[-1]                      #Get the last item in a list

for bike in bikes:                         #Looping through a list
 print(bike)

bikes = []                                 #Adding items to a list
bikes.append('trek')
bikes.append('redline')
bikes.append('giant')

squares = []                               #Making numerical lists
for x in range(1, 11):
 squares.append(x**2)
 ```
