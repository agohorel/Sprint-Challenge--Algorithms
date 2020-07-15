#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n^3)
I believe this is O(n^3) because the `while` loop is running while `a` is less than the cube of `n`, rather than just `n` which would be O(n). 


b) O(n log n) 
I believe this is O(n log n) because while there are nested loops (the `while` inside the `for` loop), the inner loop is running `while j < n`, but `j`'s value is being doubled each time giving it a log n behavior. So the first `n` is the outer for loop, and the `log n` is from the inner loop. 


c) O(n)
I believe this is O(n) beacuse it's recursive function that moves toward the base case in a linear fashion (subtracting `1` from `bunnies` each time).

## Exercise II

I would try dropping the egg from a minimal height that I can assume _will not_ break the egg, then add height (floors) using a binary search approach, doubling the floors until an egg breaks, then halving until i hit the minimum point where an egg will break. I think starting low would result in fewer broken eggs overall because you might not break your first few attempts, where if you started from the top you'd pretty much be guaranteed to break your first attempt and not really be much closer to finding the target floor. I think this approach would have an average time complexity of O(log n) due to the binary search nature of the doubling/halving approach.
