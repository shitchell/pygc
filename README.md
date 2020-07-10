# pygc
Python Google Calculator - A command line interface to Google Calculator

### About

This tool simply sends your requests to `http://suggestqueries.google.com/complete/search?output=firefox&q=`. Any response that begins with a "=" is the result of Google Calculator and thus returned.

### Usage

You can pipe data to pygc

```sh
echo '2 + 2' | pygc
```

You can use pygc with arguments as an equation

```sh
pygc '2 + 2'
```

You can use pygc interactively

```
me@localhost $ pygc
% 2 + 2
= 4
% 2 inches in meters
= 0.0508 meters
```

### Google Calculator functions and variables

```
Basic Operations:
+    (Addition)
-    (Subtraction)
/    (Division)
*    (Multiplication)
%    (Modulo)
^    (Exponentiation)
!    (Factorial)

Phrasal Operations:
th root of                   (Calculates the nth root of a number) - 5th root of 32
square root of OR sqrt       (Calculate the square root of a number) - square root of 4 OR sqrt(4)
% of                         (Calculates x% of y) - 5% of 10
X choose Y                   (Returns the number of possible permutations from choosing Y elements out of X)

Advanced Math:
sin, cos, tan                        (Trigonometric functions) - cos(pi/6)
  sec, csc, cot...
arcsin, arccos, arctan               (Inverse trigonemtric functions)
  arcsec, arccsc, arccot...
sinh, cosh, tanh                     (Hyperbolic functions)
  csch, arsinh, arccsch...
ln                                   (Base e logarithm)
log                                  (Base 10 logarithm)
lg                                   (Base 2 logarithm)
exp                                  (Exponential function) - exp(16)

Constants:
e                            (Base of the natural system of logarithms)
pi                           (3.14159265...)
i                            (Square root of -1)
gamma                        (Euler's constant)
epsilon_0                    (Electric constant)
m_e                          (Electron mass)
m_p                          (Proton mass)
c OR speed of light          (Speed of light in a vacuum)
speed of sound               (Speed of sound in air at sea level)
m_*lowercase planet name*    (Mass of each planet and the sun) m_earth...
r_*lowercase planet name*    (Radius of each planet and the sun) r_earth...

Extensive as this message is, it still manages to fail horribly. For
a more exhaustive list of Google Calculator's functions, see one or
both of the following pages:
```
http://www.googleguide.com/calculator.html

http://www.google.com/help/calculator.html
