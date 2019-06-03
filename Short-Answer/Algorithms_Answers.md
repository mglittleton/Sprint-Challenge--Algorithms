Add your answers to the Algorithms exercises here.

Exercise 1:

a) When incrementing the loop variable by n^2, the time it takes to reach n^3 is always going to be ~n. Therefore, runtime is O(n).


b) This was tricky. There are four nested loops (in order from outside):
 - first runs n times
 - second runs n-2 times
 - third runs n-4 times
 - four looks like it is dependent on n somehow, but really only runs 9 times, regardless of value of n

This means that you have three nested loops, whose runtime grows as O(n^3)

c) This recursion performs only one action for every n, so it has a runtime of O(n)


Exercise 2:

This would basically be a binary search. You would drop an egg at the middle floor. If it breaks, you would go to the middle floor between you and the ground and try again, otherwise you'd go to the middle floor between you and the roof and try again. Eventually, you'll have located the two floors where the egg breaks on the upper one or lands safely from the lower one.

The time complexity of this solution is O(log n)