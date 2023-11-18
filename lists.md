# Lists

Lists are used to store multiple data at once

```python

ages = [21, 24, 23, 23, 25]
print(ages)

```


Lists are **heterogenous datatype**

A list can store:

    - different types of data (int, float, string, list, etc)
    - duplicate values

```python

# list with elements of different data types
list1 = [1, "Hello", 3.4]

# list with duplicate elements
list1 = [1, "Hello", 3.4, "Hello", 1]

# empty list
list3 = []

```

## Accessing the elements inside the list

- positive index
- negative indexes

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

print(languages[1]) # Output: Hindi
print(languages[-3]) # Output: Hindi
```

## Slicing of a list

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

print(languages[1:2])
print(languages[::-1])
print(languages[::2])

"""
Output:

['Hindi']
['Telugu', 'Tamil', 'Hindi', 'English']
['English', 'Tamil']
"""

```


## **List are mutuable objects / datatype**

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

languages[-1] = "Malayalam"

print(languages)

```

## How to add elements to a list

1. append() - Adds an item at the end of the list

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

languages.append("Malayalam")

print(languages) # output: ['English', 'Hindi', 'Tamil', 'Telugu', 'Malayalam']

```


2. insert(index, value) - Add the element at the specified index

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

languages.insert(1, "Malayalam")

print(languages) # Output: ['English', 'Malayalam', 'Hindi', 'Tamil', 'Telugu']
```

3. extend() - To add all the items of an iterable

```python


even_num = [2,4,6,8]
odd_num = [1,3,5,7,9]

even_num.extend(odd_num) # Output: [2, 4, 6, 8, 1, 3, 5, 7, 9]

print(even_num)


```

## How to remove elements from the list

1. del statement:

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

del languages[0] 

print(languages) # Output: ['Hindi', 'Tamil', 'Telugu']

del languages 

print(languages) # Output: NameError

```


2. pop()

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

languages.pop() # it removes the last element present in the list

print(languages)

languages.pop(0) # it removes values from the specific index from the list

print(languages)

```


3. Using remove() - it removes only the first occurance of the value in the list

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu', "English"]

languages.remove("English")

print(languages) # Output: ['Hindi', 'Tamil', 'Telugu', "English"]
```

4. clear - It removes all the elements from teh list

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

languages.clear()

print(languages) #Output  []

```


## Other Methods in List

```python
languages = ['English', 'Hindi', 'Tamil', 'Telugu']

languages.reverse()

print(languages) # Output: ['Telugu', 'Tamil', 'Hindi', 'English']


numbers = [3,1,5,7,8,2]

numbers.sort() # it sorts the list in a ascending order

print(numbers)

numbers.sort(reverse=True) # it sort the list in descending order

print(numbers)

'''
Output:
['Telugu', 'Tamil', 'Hindi', 'English']
[1, 2, 3, 5, 7, 8]
[8, 7, 5, 3, 2, 1]
'''
```

## Iterating through a list

```python

languages = ['English', 'Hindi', 'Tamil', 'Telugu']

for language in languages:
    print(language)

'''
Output:

English
Hindi
Tamil
Telugu
'''

```