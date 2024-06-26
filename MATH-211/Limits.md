---
id: Limits
aliases:
  - Limits
tags: []
---
- Limit Definition(s):
    - Simple: The value that the outputs of a function approach as inputs approach a certain value
    - Preliminary: Suppose a function $f$ is defined for all $x$ near $a$ except possibly at $a$. If $f(x)$ is arbitrarily close to $L$ all $x$ sufficiently close (but not equal) to $a$, we write the following.
    $$\lim_{x \to a}=L$$
- Secant Line: a line passing through two points $(t_0, s(t_0))$ and $(t_1, s(t_1))$. The slope is given by
$$\frac{s(t_1)-s(t_0)}{t_1-t_0}$$
- Tangent Line: the line passing through $(t_0, s(t_0))$ with slope $$\lim_{t \to t_0}\frac{s(t)-s(t_0)}{t-t_0}$$
- One Sided limits:
    - Right-hand (Definition): Suppose a function $f$ is defined for all $x$ near $a$ with $x > a$. If $f(x)$ is arbitrarily close to $L$ for all $x$ sufficiently close to $a$ with $x > a$ we write
    $$\lim_{x \to a^+}{f(x) = L}$$
    - Left-hand (Definition): Suppose a function $f$ is defined for all $x$ near $a$ with $x < a$. If $f(x)$ is arbitrarily close to $L$ for all $x$ sufficiently close to $a$ with $x < a$ we write
    $$\lim_{x \to a^-}{f(x) = L}$$
    - In order for their to be a double sided limit, we must have:
    $$\lim_{x \to a^-}{f(x)} = \lim_{x \to a^+}{f(x)}$$
    - If the limits from sides are not equal, then a the double sided limit, "does not exist"
- Limits can be simplified/solved in an easier way (as compared to numerically/graphically) using [[Limit Laws]]
- Limit Example Types:
    - Tangent lines
    - Velocity
- Velocity
    - Average Veolcity
        - The average velocity over some interval $[t_0, t_1]$ is defined as
          $$v_{av} = \frac{s(t_1) - s(t_0)}{t_1 - t_0}$$
    - Instantaneous Veolcity
        - The average velocity over some interval $[t_0, t_1]$ is defined as
          $$v_{inst} = \lim_{t \to a}{v_{av}} = = \frac{s(t) - s(a)}{t - a}$$
- Solving Techniques
	- Factoring and canceling out
	- Using conjugates
		- When direct substitution is not possible, you may rationalize numerator
- See [[Limit Examples]]
