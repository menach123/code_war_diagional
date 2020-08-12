
### <a href=https://www.codewars.com/kata/5592fc599a7f40adac0000a8/train/python>Diagonals sum</a>

Create a function that receives a (square) matrix and calculates the sum of both diagonals (main and secondary)

> "Matrix = array of n length whose elements are n length arrays of integers."

3x3 example:
```
sum_diagonals([
  [ 1, 2, 3 ],
  [ 4, 5, 6 ],
  [ 7, 8, 9 ]
] ) == 30 # 1 + 5 + 9 + 3 + 5 + 7
```


```
square_matrix = [
  [ 1, 2, 3 ],
  [ 4, 5, 6 ],
  [ 7, 8, 9 ]
]
```


```
len(square_matrix)
```




    3




```
for i in range(len(square_matrix)):
    print(square_matrix[i][i])

for i in range(len(square_matrix)):
    print(square_matrix[i][(i+1)*-1])

```

    1
    5
    9
    3
    5
    7
    


```
def sum_diagonals(matrix):
    
    return sum([matrix[i][i]+ matrix[i][(i+ 1)* -1] for i in range(len(matrix))])
```


```
sum_diagonals(square_matrix)
```




    30




```

```
