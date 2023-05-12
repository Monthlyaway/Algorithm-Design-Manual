# 2 Algorithm Analysis

- RAM computation model
- asymptotic analysis of worst-case complexity
- Big O notation

## Random access machine: RAM

**Some premises:**

- simple operation takes one time step
- each memory access takes one time step
- Loops and subroutines are not considered simple operation

**Three cases:**

- The *worst-case* complexity of the algorithm is the function defined by the maximum number of steps taken in any instance of size n.
- The *best-case* complexity of the algorithm is the function defined by the min￾imum number of steps taken in any instance of size n.
- The *average-case* complexity of the algorithm, which is the function defined by the average number of steps over all instances of size n.

> We avoid all these complexities and obtaina very useful result by just considering the worst case.

## The Big Oh Notation

Functions of these three cases of complexity is rarely precise:

- Too many bumps
- Require too mach information to specify

> The Big Oh simplifies our analysis by ignoring levels of detail that do not impact our comparison of algorithms.

Some math:

$$f(n)=O(g(n)) \quad f(n)=\Omega(g(n)) \quad f(n)=\Theta(g(n))$$

upper bound, lower bound, nice bound   比较判别法

> The Big Oh notation and worst-case analysis are tools that greatly simplify our ability to compare the efficiency of algorithms.

$3 n^2-100 n+6=\Theta\left(n^2\right)$, **because both $O$ and $\Omega$ apply;**

$3 n^2-100 n+6 \neq \Theta\left(n^3\right)$, because only $O$ applies;

$3 n^2-100 n+6 \neq \Theta(n)$, because only $\Omega$ applies.
