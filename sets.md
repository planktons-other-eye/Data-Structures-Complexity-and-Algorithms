### Sets in Python

-unordered collection with no duplicate elements 

</br> 

**How to define a set:**

```python 

set1 = {1, 2, 3}
set2 = {'h', 'e', 'l', 'l', 'o'}
set3 = {7}
set4 = set()
```
</br>

**Basic membership operators:**

-a set has no duplicates 

-set membership operation is one of the fastest compares to strings, lists, tuples 

-can be certain a target exists or does not exist in our data 

```python

example = set('hello')

print(\'h\', 'h' in example) #membership of h is True
print(\'z\', 'z' not in example) #non-membership of z is True 
```
</br>

**Assigning values in a set:**

-due to unordered nature of a set, there is no concept of indexing or slicing with a set 

-however a set **is iterable**

</br>

**Python sets are mutable:**

-can add or remove values (can use .add(), .remove(), .discard(), .pop(), and .clear())

</br>

**Powering up sets: set operators:**

  * union - combining of two sets 
  * intersection - members that only exist in both sets
  * difference - members thaat only exist in first set and not second set 
  * symmetric difference - members that exist in one or the other set, but not both
  * proper subset - bool operator (A is a proper subset of B if all mebers of A are found in B, but A can't be the exact same as B)
  * subset - bool operator (A is a proper subset of B if A<B, but A can equal to B)
  * proper superset - bool operator (A is a proper superset of B if A has all the values of B and more, but are not equal to eachother)
  * superset - bool operator (A is a superset of B if A > B or A == B

</br>

**Disjoint:** a set behaviour property

-when two sets share no common value 

</br>

**Set comprehension:**

```python

def isPal(x):
  return x == x[::-1]
  
num = list(range(1, 10000))
pal_set = {num for num in nums if isPal(str(num))}

print(pal_set)
```
</br>

**Conclusion:**

-sets are sliceable or indexable

-sets can't have sets within them 

-sets do not have order, nor order of insertion

-sets can't guarantee that their values will be in order

-sets do not record a value's position








