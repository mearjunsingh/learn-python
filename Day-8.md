# Day 8

## Learning Objectives

### Sets

```python
ages = {2,3,4,9,2,1}

print(ages)
```

```python
allowed_ip = {1, 1, 2, 3, 5, 2, 9}

if ip in allowed_ip:
    print('success')
```

```python
random_tuple = (3,5,3,5,5)

random_set = set(random_tuple)

random_set.add(34)

print(random_set)

for x in random_set:
    print(x)
```


### Set Operations

```python
names = {'ram', 'shyam'}
names2 = {'shyam', 'hari'}

x = names.union(names2)
y = names.intersection(names2)
z = names.difference(names2)
aa = names.symmetric_difference(names2)

print(x)
print(y)
print(z)
print(aa)
```


## Assignment

### Problem Statement

- Create a dictionary using dictionary comprehension, where keys are numbers from 1 to 10 and values are their squares.


### Solution:

```python
ans_dict = {x:x**2 for x in range(11)}

print(ans_dict)
```