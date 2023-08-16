---
---
## Generalizing the adjustment formula

With the first half of the job done we can turn to the second half: the adjusting formula. The first simplex delimits the lower bounds, and then we progressively subtract/add the other bounds. We can notice that in the 3d6 case an additional piece of the formula "activates" when we reach each "vertex" of the possibility space. Thus we had the coefficients $$ 1,-3,3,-1 $$ for each triangle.

The keen eyed among us may have noticed that these particular numbers are the coefficients for $$ (x-1)^3 $$. They are called the [binomial coefficients](## "because we are exponentiating a linear – binomial – equation"), and are equal to $$ \binom{3}{n} \text{for } n \text{ the exponent of x} $$ We could thus rewrite our 3d6 formula in a sum like this:
$$ p_n = \sum_{k=0}^{3}*{(-1)^k \binom{3}{k} \begin{cases} 0,  & \text{for}\; n \le 6k \\ \dfrac{(n-6k)(n-6k+1)}{2}, & \text{otherwise} \end{cases}} $$

Substituting in our simplex volume formula and the summation form, it's not hard to derive the general formula for the amount of events that result in n when rolling [mdk](../../../glossary.html#ndk):
$$ num_{events} = \sum_{i=0}^{m}{(-1)^i \binom{m}{i} \begin{cases} 0,  & \text{for}\; n \le ik \\ \dfrac{(n+m-ik-2)!}{(m-1)!(n-ik-1)!}, & \text{otherwise} \end{cases}} $$