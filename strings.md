# Strings

Strings are a single / a sequence of character. For example "Hello" is a string.

```

string1 = "Hello World"
string2 = 'Python Programming'


```


## Accessing characters inside a string

We can access the characters in the string using their indexing.

1. Positive Indexing: It starts with 0 and it moves from left to right.

2. Negative Indexing: It starts from -1 and it moves from right to left.

```python

string1 = "Hello World"

# d --> -1 / 10

print(string1[-1]) # Output : d
print(string1[10]) # Output : d


```


## Slicing

Accessing the specific range of characters in a string. 

variableName[start = 0 : stop = End of the string : step = 1]


```python

string1 = "Hello World"

# Hello
print(string1[0:5])
print(string1[:5])


# Character placed at even indexes
print(string1[::2]) # Output: HloWrd

# Character placed at odd indexes
print(string1[1::2]) # Output: el ol

# Reverse the string
print(string1[::-1]) # Output: dlroW olleH
```


## Immutable Vs Mutuable Datatypes

- **Mutuable**: The values of the datatypes can be altered or changed.
- **Immutuable**: The values of the datatypes cannot be altered or changed.


## Strings are Immutable datatypes

That means the characters of a string cannot be changed.

```python

string1 = "Hello world"
string1[6] = "W"
print(string1) # Output: TypeError

string1 = "Hello world"
string1 = "Hello World"
print(string1) # Output: Hello World


```


## String Operations

1. Comparison Operator:

```python

string1 = "Hello"
string2 = "Hello"

print(string1 == string2) # Output: True

string1 = "Hello"
string2 = "hello"

print(string1 == string2) # Output: False

# Here we compare using ASCII values
print("A" < 'a') # Output : True

# to get ASCII number use ord function
print(ord("A")) # Output: 65
print(ord('a')) # Output: 97

```

2. Plus Operator (+):

```python

string1 = "Hello "
string2 = "World"

print(string1 + string2) # Output: Hello World
print(string1) # Output: Hello 
print(string2) # Output: World

```

3. Multiplication Operator (*):

```python

string1 = "Hello "
string2 = "World"


print(string1*3) # Output: Hello Hello Hello
# string1 + string1 + string1 

```

## Builtin Functions

1. len():

To find the length of the string

```python
string1 = "Hello "

print(len(string1)) #Output: 6
```

2. ord():

To find the unicode/ascii number of a character

```python

print(ord('a')) # Output: 97


```

To find the minimum value

4. max()

To find the maximum value

```python
3. min()


print(min("Hello")) # Output: H
print(max("Hello")) # Output: o

```


## String Methods

1. upper() - Converts the string to uppercase
2. lower() - Converts the string to lowercase
3. swapcase() - Converts the lowercase to uppercase and vice versa.

```python

string1 = "Hello World"

print(string1.upper())
print(string1.lower())
print(string1.swapcase())

'''
Output:

HELLO WORLD
hello world
hELLO wORLD
'''

```

4. strip, rstrip, lstrip - removes the trailling characters

```python

string1 = "----Hello-World----"

print(string1)
print(string1.strip('-'))
print(string1.rstrip('-'))
print(string1.lstrip('-'))

'''
Output:

----Hello-World----
Hello-World
----Hello-World
Hello-World----

'''


```

5. split -> breaks or slipts the string at the given character/s

```python

string1 = "Hello World Welcome to python"
print(string1.split()) # Output: ['Hello', 'World', 'Welcome', 'to', 'python']

string1 = "Hello, Welcome to python programming"
print(string1.split(',')) # Output: ['Hello', ' Welcome to python programming']

```

### To learn string formatting --> f string, .format