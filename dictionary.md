### Dictionary in Python 3

</br>

-data type that stores a collection of (key, value) pairs, each key only appears once

</br>

**Common operations:**
 1. adding a pair
 2. removing a pair 
 3. modifying an existing pair
 4. lookup of a value associated with a particular key

 </br>
 
**Defining a dictionary in python 3:**
 
 ```python 
 
sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

# There are 3 items: each with their unique addresses and value
# Accessing
print('Sammy dict:', sammy)
print('Username:', sammy['username'])
print('Online Status:', sammy['online'])
print('Follower Count:', sammy['followers'])

```
</br>

**Dictionary properties:**

   **Keys:** 

   -Must be immutable (strings, numbers, tuples, frozenset)

   -Unique; therefore, two same key values cannot exist in a single dictionary
   NEWEST CREATED ITEM with a duplicate KEY superceeds the previous declaration

   **Values:** Values of a dictionary within a key can be any data type

   </br>

**Updating a Dictionary:** 

-We can modify existing values by referencing the key

-We can add new values to a dictionary by creating a new key

-We can overwrite a value at an existing key by referencing and recreating the value for it

</br>

**Deletion with dictionary:** 

-We can delete a key hence deleting the value connected to the key

-We can empty out the entire dictionary

-We can delete the dictionary (uncommonly used)

</br>

**Membership:** can use the in and not in operators 

</br>

**Dictionary Methods:**

-Let A and B be a dictionary

-A.keys() –> Returns a sequence of keys/addresses in A

-A.values() –> Returns a sequence of item values in A

-A.items() –> Returns a sequence of key,item pairs in A

-A.get(address) –> Returns the item value at address

-A.update(B) –> Extends A with the dictionary of key,value pairs of B

</br>

**Iterating a Dictionary:**

-iterating the keys

-iterating the values

-iterating the key, value pairs by unpacking

</br>

**dict() constructor dictionary comprehension:**

```python

example_data = [
    ('one', 3),
    ('two', 3),
    ('three', 5)
]

data_dict = dict(example_data)
print('data_dict:', data_dict)
print('--')

# Dictionary Comprehension
# Goal: Take string numerals and assign them with their integer square
# - keys : string numerals
# - values: integer squares

example_data2 = ['1', '2', '3', '4', '5']

data2_dict = {x : int(x)**2 for x in example_data2}

print('data2_dict:', data2_dict)
```









  
  
  
