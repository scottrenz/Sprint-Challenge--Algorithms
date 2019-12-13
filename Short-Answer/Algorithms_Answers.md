#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  a = 0 # O(1) just calculates once no matter what
    while (a < n * n * n): # O(n2) Just calculates once but can loop quadradically
      a = a + n * n # O(1) just calculates once at a given time
b)  sum = 0 # O(1) calculates once
    for i in range(n): # O(n) can loop linearly
      j = 1 # O(1) calculates once at a given time
      while j < n: # O(n) although it calculates once, it can run linearly
        j *= 2   # O(1) calculates once in a moment
        sum += 1 O(1) calculates once in a moment
c)  def bunnyEars(bunnies): # O(1) done once
      if bunnies == 0: # O(1) done once
        return 0 # O(1) done once

      return 2 + bunnyEars(bunnies-1) # O(1) done once

## Exercise II


Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

The thing to do is drop no eggs.
This way zero are dropped and zero are broken.
zero + zero = zero
That is the minimum
Therefor, any value of f will be fine
The complexity is constant

