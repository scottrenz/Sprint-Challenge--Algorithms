#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  a = 0 # O(1) just calculates once no matter what
    while (a < n * n * n): # O(n3) Just calculates once but can loop quadradically
      a = a + n * n # O(n) just calculates once at a given time
b)  sum = 0 # O(1) calculates once
    for i in range(n): # O(n) can loop linearly
      j = 1 # O(1) calculates once at a given time
      while j < n: # O(n log n) although it calculates once, it can run linearly
        j *= 2   # O(n) calculates once in a moment
        sum += 1 O(1) calculates once in a moment
c)  def bunnyEars(bunnies): # O(1) done once
      if bunnies == 0: # O(1) done once
        return 0 # O(1) done once

      return 2 + bunnyEars(bunnies-1) # O(n) done linear

## Exercise II


Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

I am going to suppose that I have a set number of eggs.
I have a set number of floors that are equal to or less than the number of eggs.
I am required to drop all the eggs from the floors starting at top and going down one floor at a time.
I am required to drop at least one egg from each floor.

I would make a recursive module that would determine all the possilble ways that the eggs could be thrown from each floor with an eating cookies algorith.
I would make a module that would loop increasing f from floor one to the top and loop through the results throwing that number of eggs from each floor as determined from the other module and would accumulate for each of the number of ways, the number of eggs broken based on if they were above floor f or not.
I would give a result showing for each f the best strategy for breaking the least number of eggs based on finding the minumum number brokne with that f floor.
