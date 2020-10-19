# Answers to Homework 1

## Problem 1

a.

  i. \[ 3_{10} \] Explanation: \[ 1.2^0 + 1. 2^1 = 1.1 + 1.2 = 1 + 2 = 3 \]

  ii. \[ 5_{10} \]

  iii. \[ 8_{10} \]

  iv. \[ 13_{10} \]

  v. \[ 43_{10} \] 

  vi. \[ 38_{10} \]

  vii. \[ 30_{10} \]

  viii. \[ 128_{10} \]

  ix. \[ 255_{10} \]

  x. \[ 215_{10} \]

b. 

  i. \[ 111_{2} \] Explanation: \[ 7/2^2 = 1, 3/2^1 = 1, 1/2^0 = 1 \]

  ii. \[ 1010_{2} \]

  iii. \[ 100001_{2} \]

  iv. \[ 110010_{2} \]

  v. \[ 1100000_{2} \]

  vi. \[ 1101100_{2} \]

  vii. \[ 11010110_{2} \]

  viii. \[ 1111_{2} \]

  ix. \[ 1000111_{2} \]

  x. \[ 10010010_{2} \]

c.

  i. \[ 10_{2} \] Explanation: \[ 1.2^0 + 1.2^0 = 2 = 2^1 = 1.2^1 + 0.2^0 = 10_{2} \]

  ii. \[ 101_{2} \]

  iii. \[ 1001_{2} \]

  iv. \[ 11000_{2} \]

  v. \[ 100011_{2} \]


## Problem 2


a.

| A | B | C |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

b.

| A | B | C |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

c.


| A | B | C |
|---|---|---|
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 0 |

d.

| A | B | C |
|---|---|---|
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

e. 

| A | B | C |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 0 |

Explanation: 

A XOR A = 0. 
If C = A XOR B then C XOR C = 0

## Problem 3

a. 

Let **A** be the Major Street.
Let **E** be indication of Green Light on **A**
Let **B** be the Minor Street.
Let **F** be indication of Green Light on **B**

E = A
F = B AND (NOT A)

| A | B | E | F | C |
|---|---|---|---|---|
| 0 | 0 | 0 | 0 | X |
| 0 | 1 | 0 | 1 | 1 |
| 1 | 0 | 1 | 0 | 0 |
| 1 | 1 | 1 | 0 | 0 |

For C, we have the truth table. Currently, the value denoted by 
X is undefined.
if X were 1, then C = NOT A.
if X were 0, then C = F.

b.

We have chosen the approach where C = F.


![C = B AND (NOT A)](01-Diagram-TruthTable.svg)



# Problem 4

a. Searching

b. Scheduling

c. Shortest Path

# Problem 5

a.

| A | A | NOT A | A AND A | NOT (A AND A) |
|---|---|-------|---------|----------------
| 0 | 0 | 1     | 0       |    1          |
| 1 | 1 | 0     | 1       |    0          |

b.

  i.

  A NAND B = (NOT A) OR (NOT B) = C

  Now:
  
  NOT C = NOT(NOT(A AND B))
   
  So, to construct A AND B, we first NAND them. With this NAND output,
  we NAND it with itself, to yield its complement.

  ii.

  X NAND X = NOT X. See (a)


c. 

  We can do OR in a few ways, my approach is: **De Morgan's Law** allows us to do:

  NOT(A AND B) = (NOT A) OR (NOT B)

  So:

  NOT((NOT A) AND (NOT B)) = (NOT (NOT A)) OR (NOT (NOT B)) = A OR B

  So, we first use NANDs to NOT A and B individually, then we NAND these NOTs together.

d. For the Truth Table:

 Let's represent A NAND B as E

 Let's represent A NAND E as F

 Let's represent B NAND E as G

| A | B | E | F | G | C |
|---|---|---|---|---|---|
| 0 | 0 | 1 | 1 | 1 | 0 |
| 0 | 1 | 1 | 1 | 0 | 1 |
| 1 | 0 | 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 | 1 | 0 |

Now for XOR, see Problem 2 b. They are equivalent.
