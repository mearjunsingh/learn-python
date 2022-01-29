# Day 3

## Learning Objectives

### Multiple Conditional Statements

```python
gender = 'f'

if gender == 'm':
    pronoun = 'He'
else:
    pronoun = 'She'

print(pronoun, 'is a student.')
```

```python
number = -12

if number > 0:
    print('It is Positive.')
elif number < 0:
    print('It is Negative.')
else:
    print('It is Zero.')
```

```python
day = 5

if day == 1:
    print('Sunday')
elif day == 2:
    print('Monday')
elif day == 3:
    print('Tuesday')
elif day == 4:
    print('Wednesday')
elif day == 5:
    print('Thursday')
elif day == 6:
    print('Friday')
elif day == 7:
    print('Saturday')
else:
    print('Day Invalid')
```


### Control Flow

#### While Loop

```python
number = 5

while number >= 0:
    print('hello')
    number -= 1 # avoid infinite loop
```

```python
number = 2

while number >= 0:
    print(number) # variables itself can be accessed
    number -= 1
```

```python
number = int(input("Enter any number: "))
a = 1

while a <= 10:
    output = f'{number} X {a} = {number*a}'
    print(output)
    a += 1
```


#### For Loop

```python
for i in range(10, 20): # range(start, stop, step)
    print(i)
```

```python
name = "ram"

for i in name: # for each letters in string
    print(i)
```


#### `break` and `continue` keywords

```python
a = 5

while a >= -4:
    a -= 1
    
    if a == -2: # when a is -2, stop the loop
        break
    
    print(a)
```

```python
a = 5

while a >= -4:
    a -= 1
    
    if a == 2: # when a is 2, skip the current iteration
        continue
    
    print(a)
```

```python
for i in range(10, 20):
    if i == 12: # when i is 12, stop the loop
        break
    print(i)
```

```python
for i in range(10, 20):
    if i == 15: # when i is 15, skip the current iteration
        continue
    print(i)
```


## Assignment

### Problem Statement 1

- Ask user to input any number (positive only).
- Print hello number of times the user have given a number.


### Solution:

```python
number = int(input('Enter any number: '))

while number > 0:
    print('Hello')
    number -= 1
```


### Problem Statement 2

- Take any number as input from the user (positive only).
- Print Fibonacci Series upto (max, could be less sometimes) entered number (not the count, but the value itself).


### Solution:

```python
upto = int(input('Enter any number: '))
first = 0
next = 1

print(first)

while True:
    if upto <= next:
        break
    print(next)
    temp = first + next
    first = next
    next = temp
```