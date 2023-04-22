### Lesson 1: Matrices and List Comprehension

#### What is a Matrix? 

**Matrix:** representation of numbers, symbols, or expressions in a 2D array

Matrix example (mathematical): 

    A = [1 2 3 4
         5 6 7 8]
        
_let A rep matrix_


_A has m rows and n columns_

</br>

Matrix example (python): 
```python
matrix_A = [ 
    [1, 2, 3, 4],
    [5, 6, 7, 8]
]
#acessing matrix_A
print('Row 1: %s' % matrix_A[0]) #outputs [1, 2, 3, 4]
print('Value at Row 2 Column 2: %s' % matrix_A[1][1]) #outputs 6
```

#### -we have no data structure called matrix, so we program a list within a list and follow these: rules
  1. all rows must have the same number of values 
  2. all columns must have the same number of values 
  3. all items in 2D list must have the same datatypes 
  4. slice indexing starts at 0, row 1 is at matrix[0]

</br>

#### -list comprension is used when: 
  1. the list is a result of some operations applied to all its items 
  2. it is made from another iterable data
  3. list is a member of another sequence that satisfies a certain condition 

</br>

LC example 1: 
```python 
#old method
squares = []
for i in range(10):
  squares.append(i**2)
print('Our result: %s' % squares)

#lc 
squares = [i**2 for i in range(10)] 
print('Our new result: %s' % squares)
```
</br>

LC consists of: 
  * **square bracket** containing expression that describes list 
  * one or more **For clause** to explain its members 
  * none or more **if clauses** if needed

</br>

LC example 2: 
```python

#create the list: [[1, 3], [1, 4], [2, 3], [2, 1], [2, 4], [3, 1], [3, 4]] from a = [1, 2, 3] and b = [3, 1, 4]

a = [1, 2, 3]
b = [3, 1, 4]

result = [[x, y] for x in a for y in b if x != y]
print(result) 
```
</br>

LC example 3: 
```python 
#turn 2D array into single list 

vec = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]

result = [value for row in vec for value in row]
print('Vec as a single list of values: %s' % result)
```


