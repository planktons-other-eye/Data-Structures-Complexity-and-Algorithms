### Tuples in Python 3

**Tuples are:**
  * immutable 
  * allows different data types as items
  * iterable 
  * nestable 

</br>

**How to use tuples:**
  * declared with ()
  * () is an empty tuple 
  * (50,) is a singleton tuple, the comma is required (iterable data structure with only single item)
  * tuples are sliceable and indexable 
  
</br>

Tuple example: 
```python

tup = ('C', 'Java', 'Python')
empty_tup = ()
single_tup = ('Park',)

print(tup) #('C', 'Java', 'Python')
print(empty_tup) #()
print(single_tup) #('Park',)
```
</br>

**Tuple operators:** 
  1. Concatenation
  2. Reptition
  3. Membership 

</br>

_-Tuples are iterable, indexable, and sliceable_

</br>

**Built-in functions with tuple:**
  * len()
  * min()
  * max()
  * tuple()
  
</br>

**Tuple comprehension:**

```python
#tuple of even value from 1 to 100

even_tup = tuple(i for i in range(1, 101) if i % 2 == 0)
print(even_tup)
```
</br>

**Tuple packing and unpacking:**

```python
#packing

var1 = 2
var2 = 3
var3 = 5

prime = var1 + var2 + var3

print('Packed prime values are:', prime)

#unpacking and repacking 

fib = (0, 1, 1, 2, 3, 5, 8)

fib0, fib1, fibn = fib[0], fib[1], fib[2:]
print(fib0)
print(fib1)
print(fibn)
```
</br>

-packing collect multiple variable's values and assign it to a single variable 

-unpacking helps us assign certain values from a tuple to different variables 

-very useful when combines with variable arguments for function definition and function calls 


