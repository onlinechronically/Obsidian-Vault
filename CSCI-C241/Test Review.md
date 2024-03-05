- Propositional Logic
	- "Proposition"
	- Translation (English <-> Propositional Logic)
		- Implications
			- Only when/if
			- Necessary/Sufficient Conditions
		- But, Yet, However (and)
		- Exclusive vs Inclusive disjunction
- Truth assignments (Semantics)
		- Truth assignments
			- "Satisfied" (don't use true)
			- Tables
			- Satisfiable, Tautology, Contradiction, Contingency
			- Consistency
			- Logical Equivalence
			- Validity
- Proofs:
	- Natural Deduction Proofs (semi-formal)
	- Equivalence Proofs



- Examples
	1) Claim: $(R \land S) \rightarrow \neg Q, R \rightarrow S \vdash (R \land P) \rightarrow \neg (P \land Q)$
		- Goal: $(R \land P) \rightarrow \neg (P \land Q)$
		- Pf: Assume $(R \land S) \rightarrow \neg Q, R \rightarrow S$
			- Subproof
				- Assume $R \land P$
				- From $R$, we can apply $R \rightarrow S$, and conclude $S$ (application)
				- From $R$ and $S$, we can conclude $R \land S$ ($\land$ Intro)
				- From $R \land S$, we can apply $(R \land S) \rightarrow \neg Q$, and conclude $\neg Q$
				- Subproof
					- Assume $P \land Q$ towards a contradictions
					- From $P \land Q$, we can conclude $Q$ ($\land$ Elim)
				- Under the assumption of $P \land Q$, we proved $Q$ which contradicts $\neg Q$, so therefore $\neg (P \land Q)$ (Proof by Contradiction)
			- Under the assumption of $R \land P$, we proved $\neg (P \land Q)$, so therefore $(R \land P) \rightarrow \neg (P \land Q)$
	2) Claim: $A \rightarrow C, \neg \neg D, (B \lor E) \rightarrow C \vdash (A \lor B) \rightarrow (C \land D)$
		- Pf: Assume $A \rightarrow C, \neg \neg D, (B \lor E) \rightarrow C$
			- From $\neg \neg D$, we can conclude $D$ (Dbl neg)
			- Subproof
				- Assume $(A \lor B)$
				- Case 1: $A$
					- From $A$, we can apply $A \rightarrow C$, and conclude $C$ (application)
				- Case 2: $B$
					- From $B$, we can conclude $B \lor E$ (Weakening)
					- From $B \lor E$, we can apply $(B \lor E) \rightarrow C$, and conclude $C$ (application)
				- In either case of $A \lor B$, we proved $C$, so we know $C$ (Proof by Cases)
				- From $C$ and $D$, we can conclude $C \land D$ ($\land$ Intro)
			- Under the assumption of $A \lor B$, we proved $C \land D$, so therefore $(A \lor B) \rightarrow (C \land D)$ (Direct Proof)
	3) Claim: $(A \land B) \rightarrow (C \lor D) \equiv (A \rightarrow C) \lor (B \rightarrow D)$
		- Pf:
			- $(A \land B) \rightarrow (C \lor D) \equiv \neg (A \land B) \lor (C \lor D)$ (impl)
			- $\equiv (\neg A \lor \neg B) \lor (C \lor D)$ (dmg)

			- $(A \rightarrow C) \lor (B \rightarrow D) \equiv (\neg A \lor C) \lor (\neg B \lor D)$ (impl)
			- $\equiv \neg A \lor (C \lor (\neg B \lor D))$ (assoc)
			- $\equiv \neg A \lor ((C \lor \neg B) \lor D)$ (assoc)
			- $\equiv \neg A \lor ((\neg B \lor C) \lor D)$ (comm)
			- $\equiv \neg A \lor (\neg B \lor (C \lor D))$ (assoc)
			- $\equiv (\neg A \lor \neg B) \lor (C \lor D)$ (assoc)
	- An applicant will be hired only if their application is submitted on time and their file has no red flag
		- $H =$ An applicant will be hired
		- $T =$ Application submitted on time
		- $R =$ The applicant has a red flag
		- $H \rightarrow (T \land \neg R)$
		- Note: only if is reverse of if
		- $A$ if $B$ $\equiv$ $B$ only if $A$
	- $P$ is a necessary condition
		- $P$ is conclusion
	- $P$ is a sufficicient condition
		- $P$ is a premise
	- $P$ is a necessary and sufficient condition
		- $P \leftrightarrow Q$
	- Elevated levels of chemical X is a necessary condition for a positive diagnosis
		- $X =$ The levels of chemical X are elevated
		- $P =$ There is a positive diagnosis
		- $P \rightarrow X$
	- Claim: $\vdash P \lor \neg P$
		- Pf:
			- Subproof
				- Suppose towards a contradiction that $\neg (P \lor \neg P)$
					- Suppose towards a contradiction that P
					- Since $P$, we get $P \lor \neg P$ (weak)
			- We assumed $P$ and proved $P \lor \neg P$, which contradicts $\neg 