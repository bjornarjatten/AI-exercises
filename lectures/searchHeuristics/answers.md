# Exercises Lecture 5

**Theme: Search Heuristic (lecture 4)**
 
----
## Exercise 1

### Task A

$\frac{(n^2)!}{(n-1)!}$	

### Task B

$ 5^n $

### Task C

We can use the Manhattan distance on the difference between the existing location and the goal location:

$| (n - i + 1) - x_i | + | n - y_i| $

### Task D

The last heuristic is admissible, as it takes into acocunt the least steps for each car. This accounts for some cars being jump over.

## Exercise 2

### Task A

For any number n, $h_g$ will always have to take more steps than $h_1$, as it can only move to squares that are blank.
We know that $h_g >= h_1$, making $h_g$ dominant. 
This makes $h_g$ more accurate.

### Task B
$h_g$ is more accurate than $h_1$ for all cases except if there was a direct path with empty squares from the current location to the goal location.

$h_g$ is more accurate than $h_2$ if there are some filled squares on the path between the current location and the goal location.

### Task C

Count the number of moves of the following algorithm:
- Repeat until all tiles are at their goal position
    - if the blank is at the bottom right position then move a misplaced tile to its position
    - move the misplaced that has the blank as goal position, to the goal position