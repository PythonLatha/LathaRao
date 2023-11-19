# Dictionaries
 It is a collection of data that are stored as key-value pairs.


 Keys -> Should be of immutable datatypes --> Numbers, Strings, Tuples
 Value -> Can be of any datatype

 ```python
 
 captials = { "India": "Delhi", "Italy":"Rome", "England":"London"}

print(captials) # Output: {'India': 'Delhi', 'Italy': 'Rome', 'England': 'Liverpool'}
print(captials["India"]) # Output: Delhi
 ```

 ## Dictionary are heterogenous datatypes

 ```python
 
 dictionary = {
    1 : "Hello",
    (1,2) : [1,2,3],
    "Hello": {
        "key" : "value"
    }
}

print(dictionary)
print(len(dictionary))

 ```


 ## How to add values and delete values from dictionary

```python

capitals = {}

# add key value pair to the dictionary
capitals["India"] = "Delhi"
capitals["England"] = "London"

print(capitals)# Output: {'India': 'Delhi', 'England': 'London'}

# remove values from the dictionary
# 1. del statement

del capitals["India"]

print(capitals) # Output: {'England': 'London'}

# 2. clear method
capitals = {'India': 'Delhi', 'England': 'London'}
capitals.clear()
print(capitals) # Output: {}

```

## Dictionary Methods

1. keys() -> Returns list of all the keys present in the dictionary
2. values() -> Returns list of all the values present in the dictionary

```python

captials = { "India": "Delhi", "Italy":"Rome", "England":"London"}

print(captials.keys())
print(captials.values())

```

3. get(key, default value)


```python

captials = { "India": "Delhi", "Italy":"Rome", "England":"London"}

print(captials.get("USA", 0)) # Output: 0
print(captials.get("India", 0)) #Output: Delhi
```

4. items()


```python

captials = { "India": "Delhi", "Italy":"Rome", "England":"London"}

print(captials.items())

# Output: dict_items([('India', 'Delhi'), ('Italy', 'Rome'), ('England', 'London')])
```

## Iterating through for loops

```python

captials = { "India": "Delhi", "Italy":"Rome", "England":"London"}

# print key values one by one
for country in captials:
    print(country)

# Only values of the dictionary
for capital in captials.values():
    print(capital)

# Both keys and values
for key, value in captials.items():
    print(key, value)
```

## HW:

Identify two numbers from the list, which when added gives the target value

nums = [2, 11, 7, 15]
target = 9
2 + 7 --> 9

output:
[2, 7]