# CMPS 2200 Assignment 4
## Answers

**Name:**____Killian Daly_________


Place all written answers from `assignment-04.md` here for easier grading.

**1a)** Given a $N$ dollars, state a greedy algorithm for producing
as few coins as possible that sum to $N$.

Similar to how binary functions, the greedy algorithms that produces as few coins as possible for sum $N$ is to taake the
largest possible value $2^x$ that fits within $N$, over and over until you are left with 0. For example, 18 would be
represented with 2^4 & 2^1, or in binary 10010, where 1 represents a coin. 


**1b)** Prove that this algorithm is optimal by proving the greedy
  choice and optimal substructure properties.

**enter answer in `answers.md`**


**1c)** What is the work and span of your algorithm?

The $W(n)$ can be shown as $O(\log(n))$
Span is the same, as there is only one branch, $S(n)$ = $O(\log(n))$

**2a)** You realize the greedy algorithm you devised above doesn't
  work in Fortuito. Give a simple counterexample that shows that the
  greedy algorithm does not produce the fewest number of coins.
  
No the greedy algorithm does not produce the fewest coins in Fortuito. One counterexample is coins 11, 5, and 1.
In this example, the greedy scheduler would take 11+1+1+1+1 to reach 15, but the optimal selection is 5+5+5


**2b)** Since you paid attention in Algorithms class, you realize that
  while this problem does not have the greedy choice property it does
  have an optimal substructure property. State and prove this
  property.

C(X) = Min(C((i-k(subscript n)) + 1))


**2c)** Use this optimal substructure property to design a
  dynamic programming algorithm for this problem. If you used top-down
  or bottom-up memoization to avoid recomputing solutions to
  subproblems, what is the work and span of your approach?

Work using memoization would be
$O(N*k)$ due to the use of K at each level. Span would simply be $O(n)$

