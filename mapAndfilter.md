### Map and Filter in Python 3

#### Map Function:

-apply a function to an iterable data 

-map(function_name, sequence)

-function_name: any function that returns a desired value or choice 

-sequence: any iterable data type 

-map function doesn't return specific data type but instead a python iterable data, after we apply map function, we just execute list function on it 

</br>

```python 
#Example: 1

def square(num):
  '''squares the given num argument'''
  return num ** 2
  
array = list(range(1, 11))
square_array = list(map(square, array))

print("OG array:", array)
print("Array squared:", square_array) 

#Example: 2 (example of not needing the map function)

def upper(x):
  return x.upper()
  
word = 'hello world!'
upper_word = ''.join(list(map(upper, word)))

print(word) #hello world!
print(upper_word) #HELLO WORLD!
print(word.upper()) #HELLO WORLD!
```
</br>

#### Filter function: 

-filter out items from a data set that meets a certain condition

-filter(bool_returning_function, sequence) 

-function: function name provided for filter() must return bool value and should also be able to handle the items in the sequence as its arguments 

-sequence: any iterable data type 

</br>

```python

#Example 1:

def isOdd(x):
  return x % 2 != 0 
  
array = list(range(1, 101))
odds = list(filter(isOdd, array))

print('Odd numbers from 1 to 100:' odds) 

#Example 2: Palindrome 

def isPal(x):
  return x == x[::-1]
  
array = list(range(1, 10000))

pal_num = list(map(int, filter(isPal, map(str, array))))

print('Pal numbers from 1 to 10000', pal_num)
```
</br>


**Composition of functions:** idea of using functions within a function call or apply one function to the result of another function





