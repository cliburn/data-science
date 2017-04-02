
# Entrance exam for Data Science track

This exam is open book and you may use the Internet. You may use any programming tool that you like to answer the question - e.g. Unix shell commands, a programming language such as R, Python, Java etc.  

**1**. Identify the path to the file in the folder treasure_hunt that has the word "treasure" in it. Note that treasure_hunt has 10 folders each with a 100 files. (10 points)

```bash
grep -R treasure treasure_hunt
```

**2**. Count the number of times the letter `n` occurs in the file `treasure_hunt/ybmtuosizb/fqnexnotim`. Ignore case - that is, count both `n` and `N`. (10 points)

```bash
grep n -io treasure_hunt/ybmtuosizb/fqnexnotim | wc -l
```

**3**. What file in the the treasure_hunt folder has the most number of words? (10 points)

```bash
find treasure_hunt/ -type f -exec wc -w {} \; | sort -r | head -n 1
```

**4**. Implement the following algorithm (pseudocode assumes a language with 0-based arrays) and use it to sort the numbers `3,1,4,5,2` in ascending order. (10 points)

```
func my_sort( var a as array )
    for i from 1 to N
        for j from 0 to N - 1
           if a[j] > a[j + 1]
              swap( a[j], a[j + 1] )
end func
```


```python
def my_sort(A):
    n = len(A)
    for i in range(1, n):
        for j in range(n-1):
            if A[j]  > A[j+1]:
                A[j], A[j+1] = A[j+1], A[j]
```


```python
A = [3,1,4,5,2]
my_sort(A)
A
```




    [1, 2, 3, 4, 5]



**5**. How many swap operations were performed in sorting `3,1,4,5,2` using the algorithm from the previous question? What is the Big O complexity of this sorting algorithm? (10 points)


```python
def my_sort(A):
    n = len(A)
    nswaps = 0
    for i in range(1, n):
        for j in range(n-1):
            if A[j]  > A[j+1]:
                A[j], A[j+1] = A[j+1], A[j]
                nswaps += 1
    print(nswaps)
```


```python
A = [3,1,4,5,2]
my_sort(A)
```

    4


Complexity = $\mathcal{O}(n^2)$

**6**. The Fibonacci sequence is `1,1,2,3,5,8,13,21,...`. The 6th Fibonacci number is 8. Write a program to calculate the 20th Fibonacci number. (10 points)


```python
def fib(n):
    a, b = 1, 1
    for i in range(n-2):
        a, b = b, a+b
    return b
```


```python
fib(6), fib(20)
```




    (8, 6765)



**7**. Express the decimal number 3.125 as a binary number. (10 points)


```python
11.001
```




    11.001



**8**. Download the file https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data without using a browser and save it as `iris.csv` (10 points)

```bash
curl https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data -o iris.csv
```

**9**. What is the solution $x$ to the matrix equation $Ax = b$ if

$$
A = \pmatrix{1 & 2 \\3 & 4}
$$

and

$$
b = \pmatrix{5 \\ 11}
$$


```python
import scipy.linalg as la

A = np.array([[1,2],[3,4]])
b = np.array([5, 11])
la.solve(A, b)
```




    array([ 1.,  2.])



**10**. Suppose the current population of Durham is 100,000 and the population of Chapel Hill is 200,000. Every year, 10% of the people in Durham move to Chapel Hill, and 90% stay in Durham; 20% of the people in Chapel Hill move to Durham and 80% stay in Chapel Hill. Assuming no births, deaths or immigration/emigration, what is the population of Durham after many, many years? (10 points)


```python
M = np.array([[0.9, 0.1],[0.2,0.8]])
M
```




    array([[ 0.9,  0.1],
           [ 0.2,  0.8]])




```python
e, v, = la.eig(M, left=True, right=False)
```


```python
e, v
```




    (array([ 1.0+0.j,  0.7+0.j]), array([[ 0.89442719, -0.70710678],
            [ 0.4472136 ,  0.70710678]]))




```python
p = v[:, 0]/v.sum()
p
```




    array([ 0.66666667,  0.33333333])



The number of people in Durham after a long, long time is 2/3 of 300,000 = 200,000.


```python
# Brute force solution
p0 = np.array([1e5, 2e5]).reshape((1,2))
np.dot(p0, np.linalg.matrix_power(M, 100))
```




    array([[ 200000.,  100000.]])


