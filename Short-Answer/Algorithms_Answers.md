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

True = floor where egg will break
False = floor where egg will not break

- Define a function that takes in one argument that's an array of boolean values of size n.
  - Initialize variable f to -1.
  - Initialize variable low as 0.
  - Intialize variable high as n / 2.

  - Intialize a while loop. While high is greater than or equal to low,
    - Initialize a variable mid as high + low / 2.
    - Access array at midpoint
    - If array at midpoint is True,
      - If index - 1 is False,
        - Return index
      - Else if index - 1 is True,
        - high = index - 1
      - If array at midpoint is False,
        - low = index + 1

  - return the value of f.

The time complexity of this is O(log n)