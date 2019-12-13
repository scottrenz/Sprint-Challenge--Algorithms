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


