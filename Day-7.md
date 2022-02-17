# Day 7

## Learning Objectives

### Dictionaries

```python
ages = {
    'ram' : 23,
    'shyam' : 34,
    'hari' : 40
}

ages['hari'] = 25
ages['geeta'] = 34

print(ages)
print(ages['hari'])
```

```python
random_dict = {
    'name' : 'John',
    'age' : 29,
    'height' : 4.5,
    'is_male' : False,
    'hobbies' : ['hiking', 'movies', 'music'],
    'visited_places' : ('ktm', 'brt'),
    'favs' : {
        'color' : 'red',
        'place' : 'ktm'
    }
}

print(random_dict)

print(random_dict['favs']['color'])

for hobby in random_dict['hobbies']:
    print(hobby)

if random_dict['is_male']:
    print('he is male')
else:
    print('she is female')
```

```python
random_dict = {
    'name' : 'John',
    'age' : 29,
    'height' : 4.5,
    'is_male' : False,
    'hobbies' : ['hiking', 'movies', 'music'],
    'visited_places' : ('ktm', 'brt'),
    'favs' : {
        'color' : 'red',
        'place' : 'ktm'
    }
}

for item in random_dict.items():
    print(f'{item[0]} = {item[1]}')

for key, value in random_dict.items():
    print(key, value)

if 'some_key' in random_dict:
    print('yes')
else:
    print('no')

random_dict['name'] = 'Johnny'

random_dict.update({'age': 30})

random_dict.popitem()

print(random_dict)

for item in random_dict:
    print(item)

random_dict2 = random_dict.copy()
```


## Assignment

### Problem Statement

- From given dictionary, access post body.

```python
data = {
    "posts" : {
        "id" : 34,
        "content" : {
            "title" : "post title",
            "body" : 'post content'
        }
    }
}
```


### Solution:

```python
print(data['posts']['content']['body'])
```