---
---
## Enter triangle numbers

When looking at the odds for 3d6, the beginning few - 1,3,6,10 - show a familiar pattern: the [triangular numbers](https://oeis.org/A000217). T(n) is known to be [$$\dfrac {n(n+1)}{2}$$](## "I'm adjusting the indexing such that the smallest result is 1, to better plug in the formulas") . But when going further in, they begin to overestimate the result, and for the final numbers give way more – e.g. for [$$ n_{16} =1 $$](## "it's number 16 for 18 so that the series starts at 1") it predicts $$\dfrac {16(16+1)}{2} = 136 $$

![sequence of crossections of the event space of which we want to calculate the area](assets\images\Crosssections.gif)

One may notice, the discrepancy comes form the fact that certain combinations the formula would predict are, in fact, impossible. One such example is $$ 9=1+1+7 $$ as a d6 always is less than 7.