#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) Time complexity: O(n)
The while loop will only run as many times as the given input + 1.


b) Time complexity: O(n)
There's a nested loop within each iteration of the input, but it's a fraction of the
input, not the entire thing, so it isn't O(n ^ 2). It can't be O(n + k) either because
there's only one input, so this can be simplified to O(n).


c) Time complexity: O(n)
Its formatting is strange, but this is essentially a flavorized n * 2.

## Exercise II

If I understand this problem correctly,

- Define a function that takes in one argument that's an array of boolean values of size n.
  - Initialize variable f to -1.
  - Loop through each element in the boolean array:
    - On each iteration, check to see if the value is False.
      - Is it false? Set f to the index.
      - is it true? Do nothing. Go to the next iteration of the loop.

  - return the value of f.

This function will loop through an array of size n and then complete.
Its time complexity is O(n).