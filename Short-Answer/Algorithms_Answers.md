Add your answers to the Algorithms exercises here.

# Exercise I

Give an analysis of the running time of each snippet of
pseudocode with respect to the input size n of each of the following:

```
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
```
## Answer A
O(n)

if n == 1: 
The while loop would run 1 time.

if n == 2: 
The while loop would run 2 times.

if n == 3:
The while loop would run 3 times. 

And so on and so forth

The run time is linear

```
b)  sum = 0
    for i in range(n):
      i += 1
      for j in range(i + 1, n):
        j += 1
        for k in range(j + 1, n):
          k += 1
          for l in range(k + 1, 10 + k):
            l += 1
            sum += 1
```
## Answer B

O(n^3)

There are three for-loops that depend on n.  The last for-loop runs a constant of 9 times.

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```
## Answer C

O(n)

This is basically a for-loop

The function runs on the loop with the number of input bunnies so it runs n times as the number of bunnies

# Exercise II

Suppose that you have an _n_-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor _f_ or higher, and doesn't get broken if dropped off a floor less than floor _f_. Devise a strategy to determine the value of _f_ such that the number of dropped eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode and give the runtime complexity of your solution.

## Answer

I would use an approach similar to the binary search method. I would divide the floors in half, throw an egg, check to see if it is broken. If the egg did break I would search the lower half of the floors, else I would search the higher half of the floors. I would repeat this process until I found f. The runtime complexity would be equivalent to the binary search method O(log(n))