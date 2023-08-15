---
---
## First calculations

For 2d6 you could easily draw a table with the results of the roll to gain insight:

|first dice&rarr;<br>second dice&darr;|**1**|**2**|**3**|**4**|**5**|**6**|
|*1*|2|3|4|5|6|7|
|*2*|3|4|5|6|7|8|
|*3*|4|5|6|7|8|9|
|*4*|5|6|7|8|9|10|
|*5*|6|7|8|9|10|11|
|*6*|7|8|9|10|11|12|

This then would show you the odds of each result:

|2|3|4|5|6|7|8|9|10|11|12|
|1|2|3|4|5|6|5|4|3|2|1|

If you add more dice, or additional rules, or both (e.g. 4d6, drop lowest for creating characters in DnD5e) this model quickly becomes unwieldy.
An additional detriment was that my calculator, a TI-36x Pro, could not calculate such tables, so I had to find another solution.

One could naively try to calculate all the possibilities the dice could roll, but even with 3 dice you can't use a table directly, and with nested loops in a program you can see the runtime rising exponentially

| Dice(d6) | Size of event space |
| --- | --- |
| 1 | 6 |
| 2 | 36 |
| 3 | 216 |
| +1 | \*6 |

