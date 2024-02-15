[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big- $\Omega$, and big- $\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

# Proof

###### Little o definition

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

###### Big O definition

$f(n)\in O(g(n)) \iff \exists c>0, \exists n_0, \forall n\ge n_0: f(n) \leq c g(n)$ </br>

If I find an $f(n)$, $g(n)$ and $c$ that satisfies the definition of little o, particularly $f(n) < cg(n)$, then it will always satisfiy the definition of big O ($f(n) \leq cg(n)$) as well. Because $f(n) < cg(n)$ is always equal to $f(n) \leq cg(n)$. </br>

In order for little o to be satisfied, any instance of c must make $f(n) < cg(n)$ true, but for big O only one c needs to satisfy $f(n) \leq cg(n)$. So if little o is true for all c there will always be at least one c that makes big O true. </br> 

Therefore, little o always implies big O.
