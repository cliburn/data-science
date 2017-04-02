This exam is open book and you may use the internet.

**1**. Identify the path to the file in the folder treasure_hunt that has the word "treasure" in it. (10 points)

`grep -R treasure treasure_hunt`

**2**. Count the number of times the letter `n` occurs in the file `treasure_hunt/ybmtuosizb/fqnexnotim`. Ignore case - that is, count both `n` and `N`. (10 points)

`grep n -io treasure_hunt/ybmtuosizb/fqnexnotim | wc -l`

**3**. What file in the the treasure_hunt folder has the most number of words? (10 points)

`find treasure_hunt/ -type f -exec wc -w {} \; | sort -r | head -n 1`

**4**. Implement the following algorithm (pseudocode assumes a language with 0-based arrays) and use it to sort the numbers `3,1,4,5,2` in ascending order. (10 points)

```
procedure sort( A : list of sortable items )
   n = length(A)
   repeat
     swapped = false
     for i = 1 to n-1 inclusive do
       /* if this pair is out of order */
       if A[i-1] > A[i] then
         /* swap them and remember something changed */
         swap( A[i-1], A[i] )
         swapped = true
       end if
     end for
   until not swapped
end procedure
```

**5**. How many swap operations were performed in sorting `3,1,4,5,2` using the algorithm from the previous question? What is the Big O complexity of this sorting algorithm? (10 points)

**6**. The Fibonacci sequence is `1,1,2,3,5,8,13,21,...`. The 6th Fibonacci number is 8. Write a program to calculate the 20th Fibonacci number. (10 points)

**7**. Express the decimal number 3.14 as a binary number. (10 points)

**8**. Download the file http://people.duke.edu/~ccc14/jokes/smarthou.txt without using a browser. (10 points)

**9**. What is the solution $x$ to the matrix equation $Ax = b$ if

$$
A = \pmatrix{1 & 2 \\3 & 4}
$$

and

$$
b = \pmatrix{5 \\ 11}
$$

**10**. Suppose the population of Durham is 100,000 and the population of Chapel Hill is 200,000. Every year, 10% of the people in Durham move to Chapel Hill, and 90% stay in Durham; 20% of the people in Chapel Hill move to Durham and 80% stay in Chapel Hill. Assuming no births, deaths or immigration/emigration, what is the population of Durham after many, many years? (10 points)
