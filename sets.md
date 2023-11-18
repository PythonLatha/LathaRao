# Sets

Sets are collection of unique data i.e it cannot contain any duplicate values

Sets are unordered datatypes, so there is no concept of indexing


```python

id = {1,2,3,2,3}
print(id) # Output: {1, 2, 3}
print(type(id)) # Output : <class 'set'>

```

## Sets are heterogeneous datatype

```python
id = {1,2.2,True,"Hello",3}
```

## Initiating empty sets

```python

id = {}
print(type(id)) # Output: <class 'dict'>

id = set()
print(type(id)) # Output: <class 'set'>

```

## To add values to the set

1. add()

```python

id = {1,2,3}
id.add(4)
id.add(3)
print(id) # Output: {1, 2, 3, 4}

```

2. update()

```python

id1 = {1,3,5}
id2 = {2,4}

id1.update(id2)

print(id1) # Output: {1, 2, 3, 4, 5}
```

## Remove element from the set

1. discard()

```python
id = {1,2,3,4,5}

id.discard(1)

print(id) # {2, 3, 4, 5}
```


## Set Operation

1. Union

```python

a = {1,2,3,5}
b = {3,4,5,6}

print(a | b) # Ouput: {1, 2, 3, 4, 5, 6}
print(a.union(b)) # Ouput: {1, 2, 3, 4, 5, 6}

```

2. Intersection


```python

a = {1,2,3,5}
b = {3,4,5,6}

print(a & b) # Ouput: {3, 5}
print(a.intersection(b)) # Ouput: {3, 5}

```

3. Present only in a single set

```python

a = {1,2,3,5}
b = {4,6}

print(a - b) # Output: {1, 2}
print(b - a) # Output: {4, 6}
```