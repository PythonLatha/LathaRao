# Tuples


Tuples are similar to a list, but the only difference between them are tuples are immutable objects, whereas list are mutuable objects.

## Programs on Tuples

```python
marks = (1,2,3)
print(type(marks)) # Output: <class 'tuple'>

marks = (1)
print(type(marks)) # Output: <class 'int'>

marks = (1,)
print(type(marks)) # Output: <class 'tuple'>

tuple1 = (1, "Hello", 1.2, True, (1,2,3), [1,2,3])
print(tuple1) # Output: (1, 'Hello', 1.2, True, (1, 2, 3), [1, 2, 3])


tuple1 = 1,2,3
print(type(tuple1)) # <class 'tuple'>


languages = ('English', 'Hindi', 'Tamil', 'Telugu')
for language in languages:
    print(language)
```

## Difference between tuple and list:

1. Tuples are immutable and List are mutuable
2. Since tuples are immutable they are a bit faster than a list
3. Using tuples will guarantee that it remains write-protected