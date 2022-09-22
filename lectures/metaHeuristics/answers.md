# Exercises Lecture 10

**Theme: Meta Heuristic (lecture 9)**
 
----

## Exercise 1

### Task A

See solution for the whole

| **Iteration** | **Current State** |  **Obj. Value**  |                                     **Neighbors**                                    |
|:-------------:|:-----------------:|:----------------:|:------------------------------------------------------------------------------------:|
| 1             | <D, C, E, B, F>   | 4+1+3+4+7+8 = 27 | - <C, D, E, B, F> = 25 - <C, E, D, B, F> =  - <C, E, B, D, F> = - <C, E, B, F, D> =  |

### Task B

See solution

## Exercise 2

### Task A

| Current state | Best state | Action taken | Fringe | Tabu list               |
|:-------------:|:----------:|:------------:|:------:|-------------------------|
| A             | A          | -            | BC     | <>                      |
| B             | B          | a            | CFD    | < A >                   |
| D             | D          | b            | FJE    | < A, B >                |
| E             | E          | c            | J      | < A, B, D >             |
| J             | E          | f            | H      | < A, B, D, E >          |
| H             | E          | g            | G      | < A, B, D, E, J >       |
| G             | E          | h            | FI     | < A, B, D, E, J, H >    |
| F             | E          | i            | -      | < A, B, D, E, J, H, G > |

### Task B

| Current state | Best state | Action taken | Fringe | Tabu list                     |
|:-------------:|:----------:|:------------:|:------:|-------------------------------|
| A             | A          | -            | BC     | <>                            |
| B             | B          | a            | CFD    | < a >                         |
| D             | D          | b            | FE     | < a, b >                      |
| E             | E          | c            | J      | < a, b, c >                   |
| J             | E          | f            | DH     | < a, b, c, f >                |
| D             | E          | d            | F      | < a, b, c, f, d >             |
| F             | E          | o            | BG     | < a, b, c, f, d, o >          |
| B             | E          | j            | C      | < a, b, c, f, d, o, j >       |
| C             | E          | e            | AKI    | < a, b, c, f, d, o, j, e >    |
| K             | K          | n            | -      | < a, b, c, f, d, o, j, e, n > |

### Task C

No, as it is able to go back to states which we have not been before.

## Exercise 3

See solution