---
---
## Generalizing

### Other dice

Generalizing to other dice is quite easy in principle: we should just adjust the bounds where we add/subtract our functions. An example with 3d20:

$$ p_n = \dfrac {n(n+1)}{2} - 3{\begin{cases} 0,  & \text{for}\; n \le 20 \\ {\dfrac {(n-20)(n-19)}{2}}, & \text{otherwise} \end{cases}} \\ + 3{\begin{cases} 0,  & \text{for}\; n \le 40 \\ {\dfrac {(n-40)(n-39)}{2}}, & \text{otherwise} \end{cases}} - {\begin{cases} 0,  & \text{for}\; n \le 60 \\ {\dfrac {(n-60)(n-59)}{2}}, & \text{otherwise} \end{cases}} $$

### More dice

Generalizing to more dice is a bit harder: we can't just use the triangle formula again. We need to figure out the formula for the crosssection of a hypercube. The $$ -3 \text{overcounting} +3 \text{undercounting} -1 \text{overcounting, again} $$ trick also probably does not work