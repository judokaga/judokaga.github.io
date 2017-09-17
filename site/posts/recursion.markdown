---
title: Recursion Theorem
author: Judokaga
date: Sep 12, 2017
---

Theorem:
If $a$ is an element in set $X$, $f$ is a function from $X$ into $X$, and
$\omega$ is a successor set, then there is a function $u$ from $\omega$ into X
that $u(0)$ $=$ $a$, and for every $n$ in $\omega$, $u(n^+)$ $=$ $f(u(n))$.

Proof:
Consider the set $T$ of subsets of $\omega \times X$ that satisfy:  
  (1). Containing $(0, a)$,  
  (2). If it contains $(n, x)$, then it also contains $(n^+, f(x))$.  
$T$ is obviously not empty, consider the union $t$ of sets in $T$, which obviouly
satisfies (1), (2), and is a subset of $T$.  
We prove that (3) for any $(n, x)$ and $(n, y)$ in $t$, $x = y$.  
$t$ contains $(0, a)$, assume $t$ also contains some $(0, b)$ that $b \neq a$,
then a set $t' = t - (0, b)$ is also an element of $T$, which contracts $t' \in t$,
so for $n = 0$, (3) holds.  
Now assume for $n$ (3) holds. Let the ordered pair in $t$ whose first element
if $n$ be $(n, x)$, so $(n^+, f(x))$ in $t$, if there is some $(n^+, y)$ in $t$ that
$y \neq f(x)$, then the set $t''$ = t - (n^+, y)$ still satisfy (1) and (2), so $t''$
is an element of $T$, which contracts $t'' \in t$. So for n^+ (3) holds.  
Now we've proven $t$ is such a function $u$.
