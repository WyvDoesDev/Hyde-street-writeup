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
