---
---
## Fixing the extra events

If we view the whole predicted event space, we see that the extra predicted events can also be modeled with a triangle number, as seen in the illustration below

![Crosssection when the sum is 10](assets\images\0006.png)

Acknowledging this we can adjust the formula to respect the impossible events.

$$ p_n = \dfrac {n(n+1)}{2} - 3{\begin{cases} 0,  & \text{for}\; n \le 6 \\ {\dfrac {(n-6)(n-5)}{2}}, & \text{otherwise} \end{cases}} $$

Going further, we then notice that we are undercounting the green dots are subtracted twice, while they were added once.

![Crosssection when the sum is 14](assets\images\0011.png)

Thus we can once again amend our formula.

$$ p_n = \dfrac {n(n+1)}{2} - 3{\begin{cases} 0,  & \text{for}\; n \le 6 \\ {\dfrac {(n-6)(n-5)}{2}}, & \text{otherwise} \end{cases}} + 3{\begin{cases} 0,  & \text{for}\; n \le 12 \\ {\dfrac {(n-12)(n-11)}{2}}, & \text{otherwise} \end{cases}} $$

Checking the formula even outside the upper bounds, we find that it *should* give 0:

![Crosssection when the sum is 19](assets\images\0016.png)

Going even further we find that it dips in the negative: $$ n_{19} = -3 $$

![Crosssection when the sum is 21](assets\images\0019.png)

Thus we amend our formula for the last time:

$$ p_n = \dfrac {n(n+1)}{2} - 3{\begin{cases} 0,  & \text{for}\; n \le 6 \\ {\dfrac {(n-6)(n-5)}{2}}, & \text{otherwise} \end{cases}} \\ + 3{\begin{cases} 0,  & \text{for}\; n \le 12 \\ {\dfrac {(n-12)(n-11)}{2}}, & \text{otherwise} \end{cases}} - {\begin{cases} 0,  & \text{for}\; n \le 18 \\ {\dfrac {(n-18)(n-17)}{2}}, & \text{otherwise} \end{cases}} $$

Well, we will change the formula once still, but the values it provides are final.