# Day 2

## Learning Objectives

### Basic Data Types

```python
name = 'Ram' # string
age = 25 # integer
level = 3.4 # float
is_enrolled = True # boolean
phone = '98000000' # string
address = ktm # errors here because python doesn't know what ktm is
```


### Operators

#### Arithmetic Operators

```python
sum = 4 + 5 # addition
diff = 5 - 3 # subtraction
prod = 3 * 4 # multiplication
div = 10 / 4 # division
quot = 5 / 2 # quotient
rem = 5 / 2 # remainder
expo = 3 ** 3 # exponention (power)
```


#### Assignment Operators

```python
x = 5 # Assigns right side value to left side variable
x += 3 # x = x + 3
x -= 3 # x = x - 3
x *= 3 # x = x * 3
x /= 3 # x = x / 3
x //= 3 # x = x // 3
x **= 3 # x = x ** 3
x %= 3 # x = x % 3
```


#### Comparison Operators

```python
a = 5 > 3 # is greater than
a = 5 < 3 # is less than
a = 5 >= 3 # is greater than or equal to
a = 5 <= 3 # is less than or equal to
a = 5 == 3 # is equal to
a = 5 != 3 # is not equal to
```


### Conditional Statement

```python
if True: # always runs this block as it is true
    print('printing') # notice the indentation


if False: # never runs this block as it is false
    print('never prints')


if 5 >= 4: # boolean expression is required with if condition
    print('5 is greater than or equal to 4')


mark = 43 # try changing this values
if mark >= 32:
    print('passed')
else: # if condition can have optional else block 
    print('failed')


mark = 34
gender = 'm'
if mark >= 32:
    if gender == 'm': # nested if, notice the indentations
        print('He is passed')
    else:
        print('She is passed')
else:
    print('failed')
```


## Assignment

### Problem Statement 1

- Ask user to input their age.
- If age is greater than or equal to 18, print `Allowed to vote`.
- If not, print `Not allowed to vote`.


### Solution:

```python
age = int(input("Enter your age: "))

if age >= 18:
    print('Allowed to vote')
else:
    print('Not allowed to vote')
```


### Problem Statement 2

- Take two numbers from user.
- Check that number and print if it is positive or negative or zero.


### Solution:

```python
num = int(input('Enter any number: '))

if num > 0:
    print('positive number')
elif num < 0 :
    print('negative number')
else:
    print('its zero')
```