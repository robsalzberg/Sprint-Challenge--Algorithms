Add your answers to the Algorithms exercises here.

# EXERCISE I

## ANSWER A
Big O Notation

n^3 = a+n^2
a is a constant so it is dropped
n^3/n^2
Two of the three n's cancel themselves out
n = O(n)

## ANSWER B

n is multiplied by n for each of the first three loops
n+n+n
The last loop is a constant 
n+n+n+k
The constant is dropped
n^3 = O(n^3)

## ANSWER C

This is a recursive loop so it will run n bunnies until it reaches 0
Therefore Linear Time
O(n)

# EXERCISE II

## ANSWER

I would use an approach like the binary search method.  I would divide the floors in half and throw the egg to see if it breaks n/2.  If it breaks than 
f is below n/2.  If it doesn't break than f is above n/2.  I would repeat this process until f is found. Base is 2, 2/2=1. Runtime complexity is the 
same as the binary search method O(log n).
