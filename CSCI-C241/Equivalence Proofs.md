- **Chain Proof Rules**
	- **Commutative Laws**
		- $p \land q \equiv q \land p$
		- $p \lor q \equiv q \lor p$
	- **Distributive Laws**
		- $p \land (q \lor r) \equiv (p \land q) \lor (p \land r)$
		- $p \lor (q \land r) \equiv (p \lor q) \land (p \lor r)$
	- **De Morgan's Laws**
		- $\neg (p \land q) \equiv \neg p \lor \neg q$
		- $\neg (p \lor q) \equiv \neg p \land \neg q$
	- **Associative Laws**
		- $p \land (q \land r) \equiv (p \land q) \land r$
		- $p \lor (q \lor r) \equiv p \lor (q \lor r)$
	- **Material Implication**
		- $p \rightarrow q \equiv \neg p \lor q$
	- **Transitive Property**
		- If $x = y$ and $y = z$, then $x = z$
		- If $p \equiv q$ and $q \equiv r$, then $p \equiv r$
		- If $p \vdash q$ and $q \vdash r$, then $p \vdash r$
	- **Double Negation**
		- $\neg \neg p \equiv p$
	- **Idempotence Laws**
		- $p \land p \equiv p$
		- $p \lor p \equiv p$
	- **Absorption**
		- $p \lor (p \land q) \equiv p$
		- $p \land (p \lor q) \equiv p$
- **Strategy: - use eqnarry in .tex**
	1) Write both sides in terms of $\land, \lor, \neg$
	2) Push all the negations on both sides, "inside" as far as they go using **De Morgan's Laws**
	3) Choose to make the main connective on both sides, either $\land$ or $\lor$ and rewrite if needed using **Distributive Laws**

- **Other Rules**
	- Tautology ($\top$)
		- $A \lor \neg A \equiv \top$
		- $\top \land p \equiv p$
		- $\top \lor p \equiv \top$
	- Contradiction ($\bot$)
		- $A \land \neg A \equiv \bot$
		- $\bot \land p \equiv \bot$
		- $\bot \lor p \equiv p$