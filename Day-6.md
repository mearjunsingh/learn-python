# Day 6

## Learning Objectives

### List Comprehension

```python
numbers = [x for x in range(50)]

print(numbers)
```

```python
numbers = [x**2 for x in range(50)]

print(numbers)
```

```python
numbers = [x for x in range(50) if x % 2 == 0]

print(numbers)
```


### Logical Operators

```python
is_older_than_18 = True
is_in_nepal = True

if is_older_than_18 and is_in_nepal:
    print('can vote')

can_vote = is_older_than_18 or is_in_nepal

print(can_vote)

can_vote = False

print(not can_vote)
```


### Tuples

```python
ages = (34, 23, 43, 67) 

print(len(ages))

if 43 in ages:
    print('yes')

for age in ages:
    print(age)
```


### Tuple Comprehension

```python
odd_numbers = tuple(number for number in range(0, 11) if number % 2 == 1)

print(odd_numbers)
```


### Nested Lists and Tuples

```python
random_list = [
    1,
    2,
    3,
    5,
    "ram",
    "shyam",
    [
        'ktm',
        'brt',
        [
            'ktmmmmmmm'
        ]
    ]
]

random_tuple = (
    (4, 3),
    (4, 2)
)

print(random_list[6][2][0])

print(random_tuple[0][1])
```


## Assignment

### Problem Statement

- From a list of numbers from 1 to 10, find odd numbers.
- Skip number 5.
- With and without list comprehension, both.


### Solution:

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

odd_numbers = []
for number in numbers:
    if number % 2 == 1:
        if number != 5:
            odd_numbers.append(number)

odd_numbers2 = [number for number in numbers if number % 2 == 1 and number != 5]

print(odd_numbers)
print(odd_numbers2)
```