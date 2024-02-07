- They are sentences/statements that can be true/false
- **Ex (Statements/Propositions)**:
	- "The sky is blue."
	- "Truth is false."
	- "The sky is red."
	- They can an be somewhat subjective & still be a statement:
		- "Our football team is the best" => can't easily eval with logic
- **Not Propositions:**
	- Commands
		- "Go over there." => not a statements/claim, no true/false
	- Questions
		- "Is the sky blue?"
	- Exclamations
		- "Um."
	- Greetings
		- "Hello"
- **Potential Propositions:**
	- Equations (must have and equality/inequality sign)
		- x + y = 1 (Proposition)
		- x + y >= 1 (Proposition)
		- x + y (Not Proposition)
	- Computer Programs (binary statements, booleans)
		- Return True/False
		- **Warning:** Side effects + actions caused by statements
- **Atomic Propositions:** Propositions that are unable to be decomposed into multiple smaller propositions.
- **Key Terms**:
	- ¬ = not
	- p = proposition
	- ∧ = and
	- ∨ = or
	- -> = if
	- $\oplus$ = exclusive or
- **Statements Types:**
	- p∧¬ p (yields a contradiction = FALSE)
	- p∨¬ p (yields a tautology = TRUE or FALSE)
	- Tautology - Always True
	- Contradiction - Always False
- **Negation:**
	- "The sky is blue" (p), "The sky is not blue" (¬ p)
	- **TIP:** utilise negations to define propositions
	- **AVOID:** because and causality
- **Compound Propositions:**
	- These propositions can be decomposed.
	- **AND** (both conditions must be true)
		- "The sky is blue and our football team won."
			- "p and q"
			- "p∧q" -> conjunction
	- **OR** (one condition must be true, can be both though)
		- "Every day I got class or I go to the gym and do not drive."
			- p1 or p2 and not p3
			- p4 = p2 and not p3 = p2∧¬ p3
			- p1∨p4 = p1∨p2∧¬ p3
	- **XOR** (exclusive or cases, only one can be true, not both)
		- "You can have ice cream or cake but not both"
			- (p1 or p2) and not p3
			- (p1∨p2)∧¬ p3
		- "Either you win or you lose"
	- Logic used to enforce on interpretation of programming
		- IF (one is true, second must be true -> application)
			- "If the program fails it returns -1"
				- Program (succeeded) -> nothing returned
				- Program (failed) -> -1 or else
	- **Truth Table**
		- | p | q | p∧q | p∨q | p->q | p+q |
			|---|---|-----|-----|------|-----|
			| T | T |  T  |  T  |  T   |  T  |
			| T | F |  F  |  T  |  F   |  F  |
			| F | T |  F  |  T  |  T   |  T  |
			| F | F |  F  |  F  |  T   |  F  |
- **Conditional Implication:**
	- IF
		- p -> q
		- premise/condition/antecedent -> conclusion/consequent
		- p -> q rules out the possibility that (p=T, q=F)
		- IF (you are drinking alcohol), then you must be at least 21 years old.
			- A = you are drinking alcohol
			- O = age >= 21
			- A -> O
			- | A | O | A -> O    if A, then O|
				 |---|---|---------------------|
				 |T|T|T|
				 |T|F|F|
				 |F|T|T|
				 |F|F|F|
				 
	
| P | Q | P $\rightarrow$ Q |
| ---- | ---- | ---- |
| T | T | T |
| T | F | F |
| F | T | T |
| F | F | T |
|  |  |  |
			- if the A is false, it defaults to true
		- if *something*, something is a premise
		- "if ==the device is on== then it must be plugged in" = "The device must be plugged in, if ==it's on==", ==highlighted== is premise
			- "The device is on if and only if it's plugged in"
				- rules out device being on and not plugged in (O=T, P=F) no battery.
				- rules out device being plugged in but not on (O=F, P=T) no switch.
			- O = device is on
			- P = device is plugged in
			- (O -> P)∧(P -> O)
			- O <-> F = bi-conditional or bi-implication
			- The device is on if it's plugged in **and** The device is on only if it's plugged in
				- (P -> O)∧(O -> P)
			- **only if** identifies a conclusion
			- |O|P|O -> P|P -> O|(O -> P)∧(P -> O) = O <-> F|
				|-|-|-|-|-|
				|T|T|T|T|T|
				|T|F|F|T|F|
				|F|T|T|F|F|
				|F|F|T|T|T|
		- "My hair got wet because it rained" is **not** the same as "if it rained, then my hair got wet", **because implies causality**
		- **Premise Tags** (premise implies conclusion)
			- if ==something==
			- when ==something==
			- while ==something==
			- where ==something==
			- in the case that ==something==
		- **Conclusion Tags**
			- only if ==something==
			- only when ==something==
			- only in the case that ==something==
			- ==something== is a necessary condition
		- **Not implications** (not capturable fully in propositional logic)
			- therefore
			- thus
			- hence
			- so
		- ???
			- because
			- since
			- due to
		- "==something== is a sufficient condition", this is a premise
		- the presence of smoke is a necessary condition for the alarm to go off
- **Existential Claims**
	- Prove by giving an example that has some property
- **Universal Claims**
	- Prove by showing everything (in some category) has some property.
- **Logical Equivalency:** A $\land$ B $\equiv$ B $\land$ A
	- The formulas are logically equivalent if and only if every assignment that satisfies one formula also satisfies the other (and vice versa).
	- We write P $\equiv$ Q to mean P is logically equivalent to Q.
	- To prove this, we can use a truth table, universal claim
	- To disprove this, we can use a truth assignment, existential claim
	- Although the following table is incorrect, here's an example: ![[Pasted image 20240117135038.png]]
- **Consistency**
	- A set of formulas is consistent if and only if, there is an assignment that satisfies all of the formulas in the set.
	- To prove: existential, with a truth assignment that satisfies all the formula's in the set
		- This is an example of an existential universal claim
	- To disprove: universal, with a truth table that shows that there is no assignment that satisfies all of the formula's in the set
	- A $\land$ $\neg$ B
	- A $\leftrightarrow$ B
- Suppose you have an assignment that satisfies:
	- **A $\lor$ (B $\rightarrow$ C) $\land$ $\neg$ A $\land$ B**
		- if B has to be true, then C must be true
	- **$\neg$ A $\land$ B
		- A has to be false
		- B would have to be true
	- the C also has to be satisfies
	- With that being said, (A = F, B = T, C = T), that satisfies
	- Assignment consists of a set of formula's (premises) and one formula (conclusion)
		- Premises:
			- A $\lor$ (B $\rightarrow$ C)
			- $\neg$ A
			- B
		- Conclusion:
			- C
- Example for validity: ![[Pasted image 20240117141612.png]]
- **Validity**
	- Cases:
		- Assignment is valid if and only if every assignment that satisfies the premise also satisfies the conclusion.
			- Proved with a truth table, going through all the rows, showing that all that have a satisfied premise has a satisfied conclusion.
		- Assignment is not valid (invalid) if and only there exists an assignment that satisfies all the premises but not the conclusion.
			- Proved with a truth assignment, showing that a premise is satisfied, and the corresponding conclusion is not satisfied.
	- When making a table, one something in the premise is false, you can move onto the next assignment.