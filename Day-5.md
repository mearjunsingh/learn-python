# Day 5

## Learning Objectives

### Python Lists

```python
persons = ['ram', 'hari', 'ram', 'shyam']

print(persons)
```

```python
test_list = [5, 3.5, 'name'] # elements can be of mixed data type

print(test_list)
```

```python
persons = ['ram', 'hari', 'ram', 'shyam']

print(type(persons)) # <class 'list'>
print(len(persons)) # 4
```


### Accessing Elements in List

```python
persons = ['ram', 'hari', 'ram', 'shyam']

person[1] = 'john' # change the value of element at index 1

print(persons[1]) # hari
print(persons[-3]) # hari
```


### List Methods

```python
ages = [34, 23, 34, 55]

ages.insert(2, '45') # insert element at index 2
ages.append('45') # append element at the end
ages.remove(23) # remove element 23
ages.pop(2) # remove element at index 2
ages.pop() # remove last element
ages.copy() # copy the list
ages.extend([34, 23, 43]) # extend the list
ages.clear() # empty the list
```


### List Membership

```python
ages = [34, 23, 34, 55]

print(34 in ages) # True
print(45 in ages) # False

if 34 in ages:
    print('34 is present in the list')
```


### Loop through Lists

```python
ages = [34, 23, 34, 55]

# using while loop (index wise)
i = 0
while i < len(ages):
    print(ages[i])
    i += 1

# using for loop (element wise)
for age in ages:
    print(age)
```


### List Slicing

```python
ages = [34, 23, 34, 55, 65, 19, 23, 89, 34, 12]

print(ages[:3]) # [34, 23, 34]
print(ages[3:]) # [55, 65, 19, 23, 89, 34, 12]
print(ages[-1]) # 12
print(ages[-2]) # 34
print(ages[1:7:2]) # [23, 55, 19]
print(ages[::-1]) # [12, 34, 89, 23, 19, 65, 55, 34, 23, 34]
```


## Assignment

### Problem Statement 1

- Find the largest number in a list. (with and without max() function).


### Solution:

```python
ages = [34, 23, 34, 55, 65]

print('With max() function: ', max(ages))

large_number = ages[0]
for age in ages:
    if age > large_number:
        large_number = age
print('Without max() function: ', large_number)
```


### Problem Statement 2

- Reverse any list.


### Solution:

```python
ages = [34, 23, 34, 55, 65]

ages.reverse()
print('With reverse() function: ', ages)

print('With slicing: ', ages[::-1])

reverse_list = []
for element in ages:
    reverse_list.insert(0, element)
print('With looping: ', reverse_list)
```