---
id: Limit Laws
aliases:
  - Limit Laws
tags: []
---
$$\text{Assume }\lim_{x \to a}{f(x)}\text{ and }\lim_{x \to a}{g(x)}\text{ exist.}$$
The following properties hold where $c$ is a real number, and $n > 0$ is an integer.
- **Sum Rule**
  $$\lim_{x \to a}{(f(x) + g(x))} = \lim_{x \to a}{f(x)} + \lim_{x \to a}{g(x)}$$
- **Difference Rule**
  $$\lim_{x \to a}{(f(x) - g(x))} = \lim_{x \to a}{f(x)} - \lim_{x \to a}{g(x)}$$
- **Constant Multiple Rule**
  $$\lim_{x \to a}{(cf(x))} = c \lim_{x \to a}{f(x)}$$
- **Product Rule**
  $$\lim_{x \to a}{(f(x)g(x))} = (\lim_{x \to a}{f(x)})(\lim_{x \to a}{g(x)})$$
- **Quotient Rule**
  $$\lim_{x \to a}{\frac{f(x)}{g(x)}} = \frac{\lim\limits_{x \to a}{f(x)}}{\lim\limits_{x \to a}{g(x)}}\text{, provided}\lim_{x \to a}{g(x) \neq 0}$$
- **Power Rule**
$$\lim_{x \to a}{f(x)^n} = (\lim_{x \to a}{f(x)})^n$$
- **Root Rule**
$$\lim_{x \to a}{\sqrt[n]{f(x)}} = \sqrt[n]{\lim_{x \to a}{f(x)}}\text{, provided} f(x) > 0 \text{, for } x \text{ near } a \text{, if } n \text{ is even}$$
- Polynomials
    A **Polynomial** is defined as A function of the form $x_n x^n + a_{n-1} x^{n-1} + ... + a_1x + a_0$ where $n \geq 0$ is an integer
    If $p(x)$ is a polynomial then:
    $$\lim_{x \to a}{p(x)} = p(a)$$
    If $p(x)$ and $q(x)$ are polynomials and $q(a) \neq 0$ then (Direct Substitution):
    $$\lim_{x \to a}{\frac{p(x)}{q(x)}} = \frac{p(a)}{q(a)}$$
- The Squeeze Theorem
    Assume for some functions $f$, $g$ and $h$ that satisfy $f(x) \leq g(x) \leq h(x)$ for $x$ near $a$ (except possibly at $x = a$). If
    $$\lim_{x \to a}{f(x)} = \lim_{x \to a}{h(x)} = L$$
    then
    $$\lim_{x \to a}{g(x)} = L$$
    As $x \to a, h(x) \to L$. Therefore, $g(x) \to L$.
    As $x$ approaches $a$, if $f$ and $h$ approach the same value, so does $g$.
