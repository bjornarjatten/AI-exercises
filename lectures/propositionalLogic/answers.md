# Exercises Lecture 6

**Theme: Propositional Logic (lecture 5)**
 
----

## Exercise 1

### Task A

The sun shines = S

I get wet = W

It rains = R

It is summer = SU

### Task B

1. S => (R => W)
2. S => SU
3. ¬SU 
4. S => W

### Task C

    ((S => (R => W)) ^ (S => SU) ^ ¬SU) => (S => W)
≡   ((¬S V (¬R V W)) ^ (¬S V SU) ^ ¬SU) => (¬S V W)
≡   ((¬S V ¬R V W) V (¬SU ^ ¬S) V (¬SU ^ SU)) => (¬S V W)
≡   ¬((¬(S ^ R) V W) V (¬(SU V S) V (¬SU ^ SU))) V (¬S V W)
≡   (S ^ R ^ ¬W) V ((SU V S) V (¬SU ^ SU)) V (¬S V W)
≡   (S ^ R ^ ¬W) V ((SU V S) V true) V (¬S V W)
≡   (S ^ R ^ ¬W) V true V (¬S V W)
≡   true

## Exercise 2

Smoke = S, fire = f, heat = h

A. S => S ≡ ¬S V S ≡ true, and is true for all models, making it valid.
B. S => F ≡ ¬S V F, if both is true, it will be true, but if s is true and f is false, it will be false, meaning is neither valid nor unsatisfiable.
C.      (S => F) => (¬S V F)
    ≡   (¬S V F) => (¬(¬S) V ¬F)
    ≡   (¬S V F) => (S V ¬F)
    ≡   ¬(¬S V F) V (S V ¬F)
    ≡   (S ^ ¬F) V (S V ¬F)

    If f is true, and s is false, it is false, but for both true, it is true, making it not valid and unsatisfiable

D. S V F V ¬F ≡ S V true ≡ true
E.      ((S ^ H) => F) <=> ((S => F) V (H => F))
    ≡   (¬(S ^ H) V F) <=> (¬S V F V ¬H V F)
    ≡   (¬S V ¬H V F) <=> ((¬S V ¬H v F)

    As these expressions are the same, the lefthand expression will always be true for all values, meaning the expression is valid.

F.      (S => F) => ((S ^ H) => F)
    ≡   ¬(¬S V F) V (F V (¬S V ¬H))
    ≡   ¬(¬S V F) V (F V ¬S) V ¬H
    ≡   true V ¬H
    ≡   true

G.      B V D V (B => D)
    ≡   B V D V ¬B V D
    ≡   B V ¬B V D V D
    ≡   true V D V D
    ≡   true V D
    ≡   true

H:      (B ^ D) V ¬D
    
        (false ^ true) V not true
        (false) V false
        false

        
## Exercise 3

### Task A

This is true, as it says that alpha is valid only if a is true, making it true for all cases.

### Task B

This suggest that alpha is always false, so as long as this statement is true, it is correct. As false never can be true, the statement is true.

### Task C

A ⊨ B if and only if B is true in all worlds where A is true. As the statement says that A implies B, we can be sure that the statement holds.

### Task D

A is logically equivalent if they are true in the same models. This holds as the statement use biimplication, so A is true if and only if B is true or false

### Task E

If the negated B and A is not equal (which the and statement indicates), it means that they are equal, meaning that a implies b.

## Exercise 4

### Task A

¬(a => b) ^ (a ∨ b <=> (c => B))
¬(a => b) ^ ((a ∨ b) => (c => b)) ^ ((c => b) => (a ∨ b))
¬(¬a v b) ^ (¬(a ∨ b) v (¬c v b)) ^ (¬(¬c v b) v (a ∨ b))
a ^ ¬b ^ (¬a ^ ¬b v (¬c v b)) ^ (¬¬c ^ ¬b v (a ∨ b))
a ^ ¬b ^ (¬a ^ ¬b v (¬c v b)) ^ (c ^ ¬b v (a ∨ b))