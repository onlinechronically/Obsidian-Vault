1. Question One
	1. $6, 8, 10$
	2. This is not possible, as $A \subseteq \mathbb{Z}$, so $A \setminus \mathbb{Z} = \varnothing$
	3. $\{-10\}, \{-12\}, \{-66\}$
	4. $\{(s) \mid \text{the first character of } s\}$
	5. $f(n) = |n|$
2. Question Two
	1. Claim: if $D \cap B \subseteq A \setminus C$, then $D \cap E \subseteq E \setminus (B \cap C)$
	2. Pf: Choose the set $A,B,C,D,E$
		3. Choose $x \in D \cap E$
		4. Since $x \in D \cap E$, $x \in D$ and $x \in E$
		5. Case 1: $x \in B$
			1. Since $x \in D$ and $x \in B$, $x \in D \cap B$
			2. Since $x \in D \cap B$, $x \in A \setminus C$
			3. Since $x \in A \setminus C$, $x \in A$ and $x \notin C$
			4. Since $x \in B$ and $x \notin C$, $x \notin B \cap C$
			5. Since $x \in E$ and $x \notin B \cap C$, $x \in E \setminus (B \cap C)$
		6. Case 2: $x \notin B$
			1. Since $x \notin B$, $x \notin B \cap C$
			2. Since $x \in E$ and $x \notin B \cap C$, $x \in E \setminus (B \cap C)$
		7. In either case, we proved that $x \in E \setminus (B \cap C)$, so $D \cap E \subseteq E \setminus (B \cap C)$
3. Question Three
	1. $(100,5),(5.55,4.44),(1,-1),(3.14,2),(420,69)$
	2. No, because for any $x,y \in \mathbb{R}$, there exists no $x,y$ such that $x-y > 1$ and $y-x > 1$
	3. No, $3 \in \mathbb{R}$ and $\neg R(3,3)$
	4. Yes, since any $n \in \mathbb{R}$ subtracted by itself ($n-n$) is equivalent to $0$ and $0 < 1$
	5. No, for any $x,y \in \mathbb{R}$, if $x-y > 1$, no matter what, $y-x < 1$
	6. Yes, this is trivially true because there exists no $x,y \in \mathbb{R}$ where $R(x,y)$ and $R(y,x)$, so there is no $x,y$ where $R(x,y)$ and $R(y,x)$ and $x \neq y$
	7. Claim: $R$ is transitive
		1. Pf: Choose $x,y,z \in \mathbb{R}$
			1. Assume $R(x,y)$ and $R(y,z)$
				1. Since $R(x,y)$, $x-y > 1$
				2. Since $R(y,z)$, $y-z > 1$
				3. Since $x-y > 1$, $x > y$ and $x$ is greater than $y$, by more than $1$
				4. Since $y-z > 1$, $y > z$ and $y$ is greater than $z$ by more than $1$
				5. Since $x>y$ ($> 1$) and $y > z$ ($> 1$), $x > z$ and $x$ must be greater than $z$ by more than $2$
				6. Since $x$ is greater than $z$ by more than $2$, then $x - z > 2$
				7. Since $x-z > 2$, $x-z > 1$, so $R(x,z)$
			8. Under the assumption of $R(x,y)$ and $R(y,z)$, we proved $R(x,z)$, so $R$ is transitive
4. Question Four, $p \colon \verb|Str| \rightarrow \mathbb{N}$, $p(s) = (\text{\# of } \verb|A|s \text{ in } s) \cdot (\text{\# of } \verb|B|s \text{ in } s)$
	1. $p$ is not one-to-one, because $p(\verb|"ABBBB"|) = 4$ and $p(\verb|"BBABB"|) = 4$, but $\verb|"ABBBB"| \neq \verb|"BBABB"|$
	2. Claim: $p$ is onto
		1. Choose $n \in \mathbb{N}$
		3. For any $n_2 \in \mathbb{N}$, we know $n_2 \cdot 1 = n_2$
		4. Since $n_2 \cdot 1 = n_2$, we know $n = n \cdot 1$
		5. Let $s \in \verb|Str|$, where $s$ is made up of a singular $\verb|"A"|$ concatenated with $n$ $\verb|"B"|$
		6. Since $s$ is made up of $1 \cdot \verb|"A"|$  and $n \cdot \verb|"B"|$ and $1 \cdot n$, we know for any $n \in \mathbb{N}$, there exists a $s \in \verb|Str|$ where $p(s) = n$
5. Question Five
	1. Define $Q$ on $\mathbb{R}$, $\{(x,y) \mid x = y^2 + 1\}$
	3. Claim: $Q$ is antireflexive
		1. Choose $x \in \mathbb{R}$
		4. For any $n \in \mathbb{R}$, where $n_2 = n^2$, where $n_2 \geq 0$, regardless of $n$
		5. Since any number squared is positive, we know $x^2 \geq 0$
		6. Since $x^2 = x \cdot x$ and $x^2 \geq 0$, we know $x^2 \geq x$
		8. Since $x^2 \geq x$ and $x^2 \geq 0$, we know $x^2 + 1 > x$
		9. Since $x_2 + 1 > x$, we know $x^2 + 1 \neq x$, so $\neg Q(x, x)$, therefore $Q$ is antireflexive