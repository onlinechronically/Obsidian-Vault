- (Linked) Lists
- A list of $X$'s is one of:
	- $\verb|[]|$ the empty list
	- $\verb|[|first, *rest \verb|]|$
		- Where $first$ is an $x$
		- and $rest$ is a list of $X$'s
	- Others ways of notating:
		- $cons(first, rest)$
		- $first \colon rest$
		- $\verb|[|first\verb|]| + rest$
- Recursive definitions
	- $\verb|len|(L) = \begin{cases} 0 \text{ if } L = \verb|[]| \\ 1 \text{ if } rest = \verb|[]| \\ 1+\verb|len|(rest) \text{ if } L = \verb|[|first, *rest\verb|]|\end{cases}$
	- $\verb|concat|(L_1,L_2) = \begin{cases} L_2 \text{ if } L_1 = \verb|[]| \\ \verb|[|find, *\verb|concat|(rest, L_2)\verb|]| \text{ if } L_1 = \verb|[|first, *\verb|[|rest\verb|]]|\end{cases}$