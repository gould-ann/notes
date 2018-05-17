#dynamic programming 


- complex recursive programming to help reduce number of program calls
- "memo-ization"

##Rules of counting 
- Addition rule: If A and B are sets that are mutually exclusive ($A \cap B = \emptyset $)
- |$A \cup B$| = |A| + |B|
- More generally, if $A_1$, $A_2$, ... $A_k$ are all mutually exclusive, then ($A_1, \cup A_2 \cup A_k...$) = |$A_1$| + |$A_2$| + |$A_3$|... + |$A_k$|
- Product Rule: A and B are finite sets then |A x B| = |A| x |B|
- Cartesian Products...
- PIE {A}, {B} $\Rightarrow(A \cup B) = |A| + |B| - |A \cap B|$
- Arrangement Principle- suppose we have n distinct objects. Then we can arrange an arrays r of them in P(n,r) = n * (n-1) * (n-2) * (n-r+1)
- so then P(n,n) = n!
- how many arrangements of 25 people on roster to 9 people on team P(25,9)

Division Rule:
-
Consider sets A & B, define a d to 1 mapping from A to B such that exactly s elements of A get mapped to 1 element in B.
If such a mapping exsists then |A| - d|B|.

Selection Principle
-

The number of ways of selecting r objects out of n objects equals C(n,r) = $ \frac {n!}{(n-r)!r!}$ (n r) is binomial coefficient

(n n) = 1

(n 0) = 1

(n 1) = n

(n n-1) = n

(n r) = (n n-r)