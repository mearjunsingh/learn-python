# Day 1

## Learning Objectives

### Printing in a console

```python
print("Hello World")
```


### Printing Integers and Strings

```python
print(5)
print("This is String")
```


### Single quote vs Double quotes

```python
print("I'm a Human")
print('He said, "Python is amazing."')
```


### Comments

```python
# This actually is single line comment

"""
This comment
can go to
multiple lines
"""

print("Comment Section") # Or comment can lie here too
```


### Assigning Variables

```python
name = "Ram" # Notice double (or single) quotes for strings
age = 24
```


### Printing Variables

```python
print(name)
print(age)
```


### Taking Input from users

```python
name = input("Enter your name: ") # By default, input is string
age = int(input("Enter your age: ")) # String converted to integer

print(name)
print(age)
```


### Find data types

```python
random_string = "Hellllo"
random_integer = 34

print(type(random_string))
print(type(random_integer))
```


### Operations on Variables

```python
a = 5
b = 6
c = a + b
print(c) # outputs 11, because they are integers

a = '5'
b = '6'
c = a + b
print(c) # outputs 56, because they are strings

a = 5
b = '6'
c = a + b # errors here because cannot add string to integer
print(c)
```


### Type conversion

```python
a = '5'
b = int(a)
print(type(b)) # although 5 (value of a) was string, b is integer now

a = 4
b = str(a)
print(type(b)) # although 4 (value of a) was integer, b is string now

a = "ram"
b = int(a) # errors here because string data is not literal of integer
print(type(b))
```


## Assignment

### Problem Statement

- Take two numbers from user.
- Calculate Sum, Difference, Product and Division.
- Display each results.


### Solution:

```python
num_1 = int(input("Enter first number: "))
num_2 = int(input("Enter second number: "))

sum = num_1 + num_2
diff = num_1 - num_2
prod = num_1 * num_2
div = num_1 / num_2

print("Sum:", sum)
print("Diff:", diff)
print("Prod:", prod)
print("Div:", div)
```