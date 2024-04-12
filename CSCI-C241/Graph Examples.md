- Example #1 (10/04/2024):
	- $\verb|[[[], [[[],[]], []]], [[], []]]|$
- Example #2 (10/04/2024):
	- Claim: To prove that for all FBTs $T$, $P(T)$ is true
	- Pf: Structural Induction for FBTs
		- (Base Step)
			- Prove $P(\verb|[]|)$ is true
		- (Inductive Step)
			- Assume for some FBTs $T_1,T_2$ that $P(T_1),P(T_2)$ are true
			- Prove $P(\verb|[|T_1,T_2\verb|]|)$
- Example #3 (10/04/2024):
	- Claim: Every FBT has an odd number of nodes
	- Goal: $\verb|[|T_1,T_2\verb|]|$ has an odd number of nodes
	- Define $nd(T) = \text{the \# of nodes in } T$
	- Pf: Structural Induction
		- (Base Step, $T = \verb|[]|$)
			- By definition $\verb|[]|$ has $1$ node, and $1$ is odd
		- (Inductive Step, $T=\verb|[|T_1,T_2\verb|]|)$
			- Assume for some FBTs $T_1, T_2$, $T_1, T_2$ both have an odd number of nodes
			- $nd(\verb|[|T_1,T_2\verb|]|) = nd(T_1) + nd(T_2) + 1$
				- ($nd(T_1)$ and $nd(T_2)$ are both odd so $nd(T_1) + nd(T_2)$ is even, therefore $nd(T_1) + nd(T_2) + 1$ is odd)
- Example #4 (10/04/2024):
	- Define $dp(T) = \text{the depth of } T$
	- Define $dp(T) = \text{the number of leaves in } T$
	- Fact: if $log()$ is increasing, so if $x>y$, then $log(x) > log(y)$
	- Fact: $log(a \cdot b) = log(a) + log(b)$
	- Fact: $log_b(n) = x \iff b^n = x$
		- $lv(\verb|[]|) = 1$
		- $lv(\verb|[|T_1,T_2\verb|]|) = lv(T_1) + lv(T_2)$
		- $dp(\verb|[]|) = 0$
		- $dp(\verb|[|T_1,T_2\verb|]|) = max(dp(T_1), dp(T_2)) + 1$
	- Claim: For any FBT $T$, $dp(T) \geq log_2(lv(T))$
		- (Base Step, $T = \verb|[]|$)
			- $dp(\verb|[]|) = 0$
			- $lv(\verb|[]|) = 1$
			- $log_2(1) = 0$
			- $0 \geq log_2(1)$
			- $0 \geq 0$
		- (Inductive Step)
			- Assume that for some $T_1, T_2$, $dp(T_1) \geq log_2(lv(T_1))$ and $dp(T_2) \geq log_2(lv(T_2))$
			- Let $m = max(lv(T_1), lv(T_2))$
			- $dp(\verb|[|T_1,T_2\verb|]|) = m+1$
			- $log_2(lv(\verb|[|T_1,T_2\verb|]|)) = log_2(lv(T_1) + lv(T_2))$
			- Since IH, $max(dp(T_1), dp(T_2)) \geq max(log_2(lv(T_1)), log_2(lv(T_2)))$
			- 