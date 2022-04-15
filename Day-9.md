# Day 9

## Learning Objectives

### Functions

```python
def print_hello():
    print('Hello')
    print('world')
    print('!')

print_hello()
print_hello()
print_hello()
print_hello()
print_hello()
```


### Function with Arguments

```python
def add(a, b):
    print(a + b)

add(4, 5)
```


### Function with Return

```python
def add(a, b):
    return a + b

res = add(15, 40)
print(res)
```

```python
def add(a, b):
    return a + b

if add(2, 1) == 3:
    print('Test Passed')
```

```python
def parse_gender(gender):
    if gender == 'm':
        pro = 'he'
    elif gender == 'f':
        pro = 'she'
    return pro

gender = 'f'

print(parse_gender(gender), 'commented')
print(parse_gender(gender), 'messaged')
```


### *args

```python
def add(*a):
    sum = 0
    for ele in a:
        sum += ele
    return sum


print(add(3, 2, 7))
```


### Multiple Returns

```python
def randoms():
    return 1, 2, 3, 4

a, b, *c = randoms()
print(a, b, c)
```


## Assignment

### Problem Statement

- Write a function to calculate any mathematical expression. Pass parameter and also use return


### Solution:

```python
def f(x):
    # 2x^2 + 2
    return ((2 * x) ** 2 ) + 2

a = int(input('Enter any number: '))
ans = f(a)
print(ans)
```