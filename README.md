# HAS 4 Quals Hyde Street
Hyde Street was a fun little JS/TS challenge where the goal was to get a given value returned after a bunch of mathematical operations luckily these only consisted of simple math operations (multiplication, division, subtraction, addition). The program that was given to us was written in C which makes it a little bit harder but not by much, here's an example
```C
#include <stdint.h>
#include <stdbool.h>

bool quick_maths(uint32_t run) {
run = run / 13;
run = run - 236;
run = run / 6;
run = run / 10;
run = run / 9;
run = run + 13651;
run = run - 214;
run = run - 45;
run = run / 7;
run = run + 1491;
return (run == 7513);
}
```

from the above code example we can see our target number we want to get is 7513, This shouldn't be hard to get because it's only addition subtraction multiplication and division, heres how we can evaluate what number to provide to get 7513

## How to get what number we want to give quick_maths
first we want to take the number we want(in this case 75130 and plug it in and apply the inverse operation
```
run = 7513-1491 (6022)
run = 6022 * 7 (42154)
run = 42154 + 45 (42199)
run = 42199 + 214 (42413)
run = 42413 - 13651 (28762)
run = 28762 * 9 (258858)
run = 258858 * 10 (2588580)
run = 2588580 * 6 (15531480)
run = 15531480 + 236 (15531716)
finally, run = 15531716 * 13 (201912308)
```
So we want to initate quick_maths with run being 201912308

