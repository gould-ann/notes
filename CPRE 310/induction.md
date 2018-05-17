# induction

assuming cases 

1) induction hypothesis

2) induction step 

- prove base cases 
- assume that the statement is true for some _k_ (induction hypothesis)
- use this to show that the statement is true for _k+1_ (induction step)
- conclude via mathematical induction that _P(n)_ is true for all n.

## Proof: (mathematical induction)

0 + 1 + 2 + ... + n = n(n+1)/2

(base-case)

left hand side = 0

right hand side = 0(0+1)/2  = 0

##### induction hypothesis:

Assume that 0 + 1 + 2 + ... + k = k(k+1)/2

##### induction step:

0 + 1 + 2 + ... + k + k + 1 = $k(k+1)/2 + k+1 $

$= (k+1)[k/2 + 1]$

$= [(k+1)(k+2)]/2$

######conclusion:

by induction, the statement is true for all n.

####another proof:

n = 0

0 + 0 + 42 = 42 which is even.

(induction hyp) assume that for some k, $k^{2} + k + 42$ is even

(induction step) $(k+1)^{2} + (k+1) + 42$

$= k^2 + 2k + k + 1 + 42 $

$= k^2 + k +42 + 2k + 2$ _(both are even)_

$\rightarrow (k+1)^2+k+1+42$ is even

##horses!!!

######Claim:
all horses in the world are of the same color

######proof:

P(n) any set of n horses in the world are of the same color, then P(n) is true for all n/

(base case) n = 1 is trivally true

#more on induction (day 2)
###questions 
 - is the statement of the form "For all n, both..."
 - Is the statement true for the first few base cases (n = 0, n = 1...)
 - if true for n = t, can you use this to prove that its true for n = k + 1

 ##examples :
 Claim 1 + r + r^2 + r^n = r^(n+1)/ (r-1)
 
 Proof:
 
 Because n = 0, the lefthand side is = 1, righthand side = r^(0+1)-1/r-1 = r-1/r-1 = 1
 
 **induction hypothesis 
 
 Assume that $$1 + rt ... + r^k = r^{k+1}-1/(r-1)$$

**induction step

add k+ 1 on both sides

1 + r + $r^2... r^{k+1} = r^{k+1}-1/(r-1) + r^k+1$

**simplify this out a bit

goes to: $r^{k+2}-1/(r-1)$

Claim: let $(x_u, y_y)$ b ethe position of the robot at the time instant n. Then $x_n + y_n$ is even for all n. 

Proof: We prove this with induction.

Base Case: n= 0 $(x_0,y_0) = (0,0)$

Hypothesis: Suppose $x_k + y_k$ is even for some k

Induction step: Proof by cases!! woot!

Use proof by cases as induction step... And then you can assume from there that all cases hold true 

**hint for induction... If there is anything recursive related 

##Strong induction

A way to prove using induction but in a stronger sense.

#####Example

Claim: Every number has a binary representation

Proof: (by induction) For every n, n has a binary representation 

Base Case: n = 0... $0 * 2^0$

Hypothesis (Strong induction) Assume that the statement is true for all n up to k. n = 1 n = k all have binary representation.

Induction Step: Assume k + 1 (use proof by cases)

Then you can assume from there!

#####Another Example

Suppose we have two types of postage stamps worth 10 cents and 15 cents. Then we can make any amount >= 10 cents that is a multiple of 5 cents.

Claim: for any amount that is 5n cents (for n > 2), this payment can be made using 10 cent and 15 cent stamps 

Proof: We proof this by using strong induction.

(Base Cases) n = 2, n = 3 are obvious (use 1 stamp each)

Induction

5(k+1) = 5k+5

= 5k-5 + 10

= 5(k-1) + 10... (as long as you can derive to k+1 in some way)

Any solution to 5(k-1) cents can be used to obtain a solution 5(k+1) cents by adding 1 10 cent stamp.

By Induction, 5n can be made for any n.