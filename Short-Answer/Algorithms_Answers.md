#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)
     the loop runs as long as a is less than n^3. a then increases with n^2 with each loop. 

        n^3 / n^2 = n



b) O(n log n)
    The outer loop runs n times. The inner loop runs log n as j is doubled each run.

        n * log n = n log n


c) O(n) 
    It is linear because the function will run for each bunny

## Exercise II
Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

I would use a binary search which has a runtime of o(log n).

I would first drop the egg for the floor in the middle. 
If the egg is broke
    I would move to the middle of the lower floors 
    drop again
If the egg did not break
    I would move to the middle of the upper floors
    drop again

I would repeat this process until I find the highest floot the egg doesnt break. This would be f. 

