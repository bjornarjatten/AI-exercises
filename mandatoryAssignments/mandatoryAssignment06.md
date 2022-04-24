# Mandatory Assignment 6

**Name:** Bjørnar Haugstad Jåtten \
**ITU-username:** bjja@itu.dk

------------------

## Task 1

To reduce the domains of the variables of W, such that W becomes arc consistent, we need to enforce thtat the variables of the domain actually is reffering to something. Below is the reduced domains:

D<sub>1</sub> = {1,2}, D<sub>2</sub> = {5,7,8}, D<sub>3</sub> = {2,4}, D<sub>4</sub> = {0,2,4}, D<sub>5</sub> = {1,2};

## Task 2

As stated during the lecture, a solution is an assignment that satisfies all of the constraints. Such an solution for W can be: 

X<sub>1</sub> = 2, X<sub>2</sub> = 8,
X<sub>3</sub> = 4,
X<sub>4</sub> = 0,
X<sub>5</sub> = 1

## Task 3

An algorithm that could find a solution to an arbitrary binary CSP could look something like this, with an ordered queue as input:

1. For all of the elements in the ordered queue, we call *REVISE*. With each call to *REVISE* we spare the elements in a new queue.
2. This new queue will now be a negation of the original queue, and will be used as an input when we go trough all of the elements once again, calling *REVISE*. This ensures that we upheld the constraints.
3. While traversing trough the negated queue, we assign a value to each of the elements in the queue.

The elements in the queue represents all of the nodes in a tree. By going trough the ordered queue, we first go from parent to child, and then, with the negated queue, we go from child to parent. This approach of first going from parent to child, and then back, ensures that we achieve polynomial time.