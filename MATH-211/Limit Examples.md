---
id: Limit Examples
aliases:
  - Limit Examples
tags: []
---
# Limit Examples
- (Describing Limits) As $x$ approaches $3$, $x^2$ approaches $9$
$$\lim_{x \to 3}{x^2 = 9}$$
- (Common Use) Values that are undefined can still have limits, given a graph $G$ where $f(3) = \text{undefined}$ ($f(3)$ is a hole), the following limit is valid:
$$\lim_{x \to 3}{f(x) = 4}$$
- Calculating Limits Numerically:
    - $f(x) = \frac{x^3-1}{x-1}$
        
      |0.9 |0.99  |0.999   |0.9999    |
      |----|------|--------|----------|
      |2.71|2.9701|2.997001|2.99970001|
      
      |1.1 |1.01  |1.001   |1.0001    |
      |----|------|--------|----------|
      |3.31|3.0301|3.003001|3.00030001|
        
      As $x$ approaches $1$, $f(x)$ approaches $3$: $\lim\limits_{x \to 1}{\frac{x^3-1}{x-1}} = 3$
- Calculating One-sided limits:
    - $g(x) = \frac{x^3 - 4x}{8|x-2|}$

      |1.9     |1.99      |1.999       |1.9999       |
      |--------|----------|------------|-------------|
      |−0.92625|−0.9925125|−0.999250125|−0.9999250013|

      |2.1    |2.01     |2.001      |2.0001     |
      |-------|---------|-----------|-----------|
      |1.07625|1.0075125|1.000750125|1.000075001|

      $$\lim_{x \to 2}{g(x)} = \text{Does not exist}$$
      $$\lim_{x \to 2^-}{g(x)} = -1$$
      $$\lim_{x \to 2^+}{g(x)} = 1$$
- Calculating piecewise function limits
    - $f(x) = \begin{cases}3 - x \text{ if } x < 2 \\ x - 1 \text{ if } x > 2 \end{cases}$
      $a = 2$

      |1.9|1.99|1.999|1.9999|
      |---|----|-----|------|
      |1.1|1.01|1.001|1.0001|

      |2.1|2.01|2.001|2.0001|
      |---|----|-----|------|
      |1.1|1.01|1.001|1.0001|

      Explanation: Since $f(2)$ is not defined within the piece wise function, a graph representing this function would have a whole where $x = a$ and have two lines with inverse slopes
          
      $$f(a) = \text{undefined}$$
      $$\lim_{x \to a}{f(x)} = 1$$
      $$\lim_{x \to a^-}{f(x)} = 1$$
      $$\lim_{x \to a^+}{f(x)} = 1$$
- Limit Laws
    - Problem 1:
        - Definitions:
          $\lim\limits_{x \to 3}{f(x)} = 2$
          $\lim\limits_{x \to 3}{g(x)} = -1$
          $\lim\limits_{x \to 3}{h(x)} = 6$
        - Problems:
            - Sub-Problem 1: Sum, Constant Multiple
              $$\begin{eqnarray}
              \lim_{x \to 3}{(f(x) + 2g(x))} &=& \lim_{x \to 3}{f(x)} + \lim_{x \to 3}{2g(x)} \\
              &=& \lim_{x \to 3}{f(x)} + 2(\lim_{x \to 3}{g(x)}) \\
              &=& 2 + 2(-1) \\
              &=& 0 \\
              \end{eqnarray}$$
            - Sub-Problem 2: Quotient
              $$\begin{eqnarray}
              \lim_{x \to 3}{\frac{h(x)}{g(x)}} &=& \frac{\lim\limits_{x \to 3}{h(x)}}{\lim\limits_{x \to 3}{g(x)}} \\
              &=& \frac{6}{-1} \\
              &=& -6 \\
              \end{eqnarray}$$
            - Sub-Problem 3: Quotient, Root, Difference
              $$\begin{eqnarray}
              \lim_{x \to 3}{\frac{h(x)}{\sqrt{f(x) - g(x)}}} &=& \frac{\lim\limits_{x \to 3}{h(x)}}{\lim\limits_{x \to 3}{\sqrt{f(x) - g(x)}}}\\
              &=& \frac{\lim\limits_{x \to 3}{h(x)}}{\sqrt{\lim\limits_{x \to 3}{(f(x) - g(x))}}} \\
              &=& \frac{\lim\limits_{x \to 3}{h(x)}}{\sqrt{\lim\limits_{x \to 3}f(x) - \lim\limits_{x \to 3}g(x)}} \\
              &=& \frac{6}{\sqrt{2 + 1}} \\
              &=& \frac{6}{\sqrt{3}} \\
              &=& 2 \sqrt{3}
              \end{eqnarray}$$
    - Problem 2:
        $$\begin{eqnarray}
            \lim_{x \to 1}{\frac{3x^2 - 7x + 1}{x + 2}} &=& \frac{3(1)^2 - 7(1) + 1}{1 + 2} \\
            &=& \frac{3 - 7 + 1}{1+2} \\
            &=& \frac{-3}{3} \\
            &=& -1
        \end{eqnarray}$$
    - Problem 3:
        $$\begin{eqnarray}
            \lim_{x \to 4}{\frac{\left ( \frac{1}{x} - \frac{1}{4} \right )}{x - 4}} &=& \lim_{x \to 4}{\frac{\left ( \frac{4}{4x} - \frac{x}{4x} \right )}{x - 4}} \\
            &=& \lim_{x \to 4}{\frac{\left ( \frac{4 - x}{4x} \right )}{x - 4}} \\
            &=& \lim_{x \to 4}{\frac{\left ( \frac{4 - x}{4x} \right )}{\left ( \frac{x - 4}{1} \right )}} \\
            &=& \lim_{x \to 4}{ \left (\frac{4 - x}{4x} \right ) \left (\frac{1}{x-4} \right )} \\
            &=& \lim_{x \to 4}{\frac{4 - x}{4x(x - 4)}} \\
            &=& \lim_{x \to 4}{\frac{-(-4 + x)}{4x(x - 4)}} \\
            &=& \lim_{x \to 4}{\frac{-(x - 4)}{4x(x - 4)}} \\
            &=& \lim_{x \to 4}{\frac{-1}{4x}} \\
            &=& \lim_{x \to 4}{\frac{-1}{4(4)}} \\
            &=& -\frac{1}{16}
        \end{eqnarray}$$
    - Problem 4:
        $$\begin{eqnarray}
            \lim_{x \to 9}{\frac{x - 9}{\sqrt{x} - 3}} &=& \lim_{x \to 9}{\frac{x - 9}{\sqrt{x} - 3} \cdot \frac{\sqrt{x} + 3}{\sqrt{x} + 3}} \\
            &=& \lim_{x \to 9}{\frac{(x - 9)(\sqrt{x} + 3)}{(\sqrt{x} - 3)(\sqrt{x} + 3)}} \\
            &=& \lim_{x \to 9}{\frac{(x - 9)(\sqrt{x} + 3)}{x - 9}} \\
            &=& \lim_{x \to 9}{\sqrt{x} + 3} \\
            &=& \sqrt{9} + 3 \\
            &=& 3 + 3\\
            &=& 6
        \end{eqnarray}$$
    - Problem 5:
        $$1 - \frac{x^2}{2} \leq \cos{x} \leq 1$$
        $$\begin{eqnarray}
            \lim_{x \to 0}{\left ( 1 - \frac{x^2}{2} \right )} &=& 1 - \frac{0^2}{2} \\
            &=& 1 - 0 \\
            &=& 1 \\
            &=& \lim_{x \to 0}{1} \\
            \lim_{x \to 0}{\cos{x}} &=& 1 \hspace{1cm} \text{(By the Squeeze Theorem)}
        \end{eqnarray}$$
    - Problem 6:
        $$\begin{eqnarray}
            \lim_{x \to 0}{\sin{x}} &=& 0 \hspace{0.5cm} \text{(By the Squeeze Theorem)} \\
            \lim_{x \to 0}{\cos{x}} &=& 1 \hspace{0.5cm} \text{(By the Squeeze Theorem)}
        \end{eqnarray}$$

        $$\begin{eqnarray}
            %%\lim_{x \to 0}{\frac{\sin{2x}}{\sin{x}}} &=& \frac{\lim\limits_{x \to 0}{\sin{2x}}}{\lim\limits_{x \to 0}{\sin{x}}} \\ %%
            \lim_{x \to 0}{\frac{\sin{2x}}{\sin{x}}} &=& \lim_{x \to 0}{\frac{2 \sin{x} \cos{x}}{\sin{x}}} \\
            &=& \lim_{x \to 0}{2 \cos{x}} \\
            &=& 2 \lim_{x \to 0}{\cos{x}} \\
            &=& 2 \cdot 1 \\
            &=& 2
        \end{eqnarray}$$
    - Problem 7 (Section 2.1, Related Exercise 13):
	    - Hint: use the secant line slope formula
		    $$s(t) = -16t^2 + 128t$$
		- $[1, 4]$
			$$\frac{256 - 112}{4 - 1} = \frac{144}{3} = 48$$
		- $[1, 3]$
			$$\frac{240 - 112}{3 - 1} = \frac{128}{2} = 64$$
		- $[1, 2]$
			$$\frac{192 - 112}{2 - 1} = \frac{80}{1} = 84$$
		- $[1, 1 + h]$, where $h > 0$ is a real number
			$$\frac{112 + -16h^2 + 128h - 112}{1 + h - 1} = \frac{-16h^2 + 128h}{h} = -16h + 128 = 16(-h + 6)$$
	- Problem 8 (Section 2.1, Related Exercise 15):
		- Hint: we use the slope formula for the secant line, and the relationship is referring to the interval
		$$s(t) = -16^t + 100t$$
		- To Do: Sketch a graph of $s$ with the secant line passing through $(0.5, s(0.5))$ and $(2, s(2))$
			$$\begin{eqnarray}
			\frac{s(t_1) - s(t_0)}{t_1 - t_0} &=& \frac{s(2) - s(0.5)}{2 - 0.5} \\
			&=& \frac{136 - 46}{1.5} \\
			&=& \frac{90}{1.5} \\
			&=& 60
			\end{eqnarray}$$
			The slope of this secant line, through the lens of average velocity could be viewed as the average velocity over the interval $[0.5, 2]$
	- Problem 9 (Section 2.1, Related Exercise 17):
		- $$s(t) = -16t^2 + 128t$$

		  |$[1,2]$|$[1,1.5]$|$[1,1.1]$|$[1,1.01]$|$[1,1.001]$|
		  |-------|---------|---------|----------|-----------|
		  |$80$   |$88$     |$94.4$   |$95.84$   |$95.984$   |

         $$v_{inst} = \lim_{t \to 1}{s(t)} = 96$$
	- Problem 10 (Section 2.1, Related Exercise 19):
		- $$s(t) = -16t^2 + 100t$$

		  |$[2,3]$|$[2.9,3]$|$[2.99,3]$|$[2.999,3]$|$[2.9999,3]$|
		  |-------|---------|----------|-----------|------------|
		  |$20$   |$5.6$    |$4.16$    |$4.016$    |$4.002$    |

         $$v_{inst} = \lim_{t \to 3}{s(t)} = 4$$
