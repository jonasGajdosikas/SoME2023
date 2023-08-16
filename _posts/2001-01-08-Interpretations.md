---
---
## Interpretations
### How do we interpret the simplex volume formula?

$$ V_n(m) = \binom{n+m-1}{n} $$ 

I can remember having seen this formula in a [Numberphile video](https://youtu.be/UTCScjoPymA). It's interpretation is as taking m-1 steps and switching n times.

Thus I propose the following procedure: we have the dimensions in some order (it does not matter, but has to be consistant) with "skipping" prepended to the list. Then we start at the "lowest" corner and step $$ m-1 $$ times in the specified dimension; and switch n times to a new direction. This procedure allows us to get a [bijection](../../../glossary.html) between each sphere in the simplex and a random permutation of $$ n $$ elements of one type and $$ m-1 $$ of a second.

### Interpretation of the dice formula

We could describe the odds of ndk as the 0-based coefficients of $$ (\sum_{i=0}^{k}{x^i})^n $$ with the caveat that this may be difficult to compute directly.

For the occasions where we want to calculate the odds for the whole possibility range, it is probably more practical to use convolutions as described in 3b1b's [video](https://youtu.be/KuXjwB4LzSA), where you succesively add additional dice until you reach the desired amount