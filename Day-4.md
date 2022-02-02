# Day 4

## Learning Objectives

### Python Strings

```python
print('This is a string')
```

```python
country = 'United States of America'

print(country)
```

```python
paragraph = '''
lorem ipsum is a random
text used as a
placeholder.
'''

print(paragraph)
```



### Escape Sequencess

```text
\n - New Line
\t - Tab
\\ - Backslash
\' - Single Quote
\" - Double Quote
\a - ASCII Bell
\f - ASCII Formfeed
\v - ASCII Vertical Tag
```


#### Examples

```python
text = "He said, \"i\'m learning python\""

print(text)
```

```python
student_record = 'Name: Ram\nAge: 25\nAddress: KTM'

print(student_record)
```

```python
notification = 'With sound\a'

print(notification)
```


### String Methods

```python
text = 'ram'
x = text.capitalize()
print(x) # Ram
```

```python
text = 'united states'
x = text.title()
print(x) # United States
```

```python
text = 'ram'
l = len(text)
print(l) # 3
```

```python
text = 'RAm'
l = text.lower()
print(l) # ram
```

```python
text = 'ram'
l = text.islower()
print(l) # True
```

```python
text = 'ram'
l = text.upper()
print(l) # RAM
```

```python
text = 'ram'
l = text.isupper()
print(l) # False
```

[Reference on Python String Methods](https://www.w3schools.com/python/python_ref_string.asp)


### String Indexes

```python
text = 'kathmandua'

print(text[0]) # k
print(text[1]) # a
print(text[2]) # t
```


### For Loop with String

```python
name = 'kathmandu'

for i in name: # for each letters in string
    print(i)
```


### String Slicing

```python
text = 'kathmandu'
x = text[1:3]
print(x) # at

print(text[:3]) # kat
print(text[3:]) # hmandu
print(text[-1]) # u
print(text[-2]) # d
print(text[1:7:2]) # aha
print(text[::-1]) # udnamhtak
```


## Assignment

### Problem Statement 1

- Ask user to input any string.
- Find the length of that string (with and without len() function).


### Solution:

```python
text = input("Enter any text: ")

print('With len() function: ', len(text))

count = 0
for letter in text:
    count += 1
print('Without len() function: ', count)
```


### Problem Statement 2

- Reverse any string after taking input from user (With and without slicing).


### Solution:

```python
text = input("Enter any text: ")

print('With slicing: ', text[::-1])

reverse_text = ''
for letter in text:
    reverse_text = letter + reverse_text
print('Without slicing: ', reverse_text)
```


### Problem Statement 3

- Convert each and every letter 'A' tp capital letter in a string (with and without replace() function).


### Solution:

```python
text = input("Enter any text: ")

print('With replace() function: ', text.replace('a', 'A'))

replaced_text = ''
for letter in text:
    if letter == 'a':
        replaced_text += letter.upper()
    else:
        replaced_text += letter
print('Without replace() function: ', replaced_text)
```