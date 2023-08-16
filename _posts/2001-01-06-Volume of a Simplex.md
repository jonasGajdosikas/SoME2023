---
---
## Volume of a crosssection of a hypercube

One may notice that for a while the crossection of a hypercube is a tetrahedron (a d4 for the dice nerds); and further speculate that the crosssection of an [n-hypercube](## "a hypercube in n dimensions") the crossection would be an [n-1-simplex](https://en.wikipedia.org/wiki/Simplex).

Thus the goal would be to first find a formula for the amount of spheres stacked in an n-simplex of side length m.

We define a series $$ V_n(m) $$ to be the number of spheres in said simplex. Then from the observation $$ V_n(m) = V_n(m-1) + V_{n_1}(m) $$ and the observations $$ V_n(1) = 1 $$ and $$ V_0(m) = 1 $$ we can postulate that $$ V_n(m) = \binom{n+m-1}{n} $$

### Proving our claim by induction

For our base cases we get:
$$ V_n(1) = \binom{n+1-1}{n} = \binom{n}{n} = \dfrac{n!}{n!(n-n)!} = \dfrac{1}{0!} = 1 $$
and 
$$ V_0(m) = \binom{0+m-1}{0} = \dfrac{(m-1)!}{0!(m-1)!} = 1 $$

The relating case is a bit longer to prove:
$$ V_n(m-1) + V_{n-1}(m) =\\ \binom{n+m-1-1}{n} + \binom{n-1+m-1}{n-1} =\\ \dfrac{(n+m-2)!}{n!(m-2)!} + \dfrac{(n+m-2)!}{(n-1)!(m-1)!} =\\ \dfrac{(m-1)(n+m-2)!}{n!(m-1)!} + \dfrac{n(n+m-2)!}{n!(m-1)!} =\\ \dfrac{((m-1)(n+m-2)!) + (n(n+m-2)!)}{n!(m-1)!} =\\ \dfrac{(n+m-2)!(n+m-1)}{n!(m-1)!} =\\ \dfrac{(n+m-1)!}{n!(m-1)!} = \binom{n+m-1}{n} = V_n(m) \qquad \blacksquare $$