**Logical Equivalence:** 
		Compound propositions that have the same truth values in all possible cases are called logically equivalent.
				The compound propositions  and  are called logically equivalent if  ↔  is a tautology. 
				The notation  ≡  denotes that  and  are logically equivalent
				
				| p   | q   | ¬p  | ¬q  | p ∨ q | ¬(p ∨ q) | ¬p ∧ ¬q |
				| --- | --- | --- | --- | ----- | -------- | ------- |
				| F   | F   | T   | T   | F     | T        | T       |
				| F   | T   | T   | F   | T     | F        | F       |
				| T   | F   | F   | T   | T     | F        | F       |
				| T   | T   | F   | F   | T     | F        | F       |


| Equivalences  | Name                | Equivalences                    | Name              |
| ------------- | ------------------- | ------------------------------- | ----------------- |
| p ∧ T ≡ p     | Identity Laws       | (p ∨ q) ∨ r ≡ p ∨ (q ∨ r)       | Associative Laws  |
| p ∨ F ≡ p     |                     | (p ∧ q) ∧ r ≡ p ∧ (q ∧ r)       |                   |
| p ∨ T ≡ T     | Domination Laws     | p ∨ (q ∧ r) ≡ (p ∨ q) ∧ (p ∨ r) | Distributive Laws |
| p ∧ F ≡ F     |                     | p ∧ (q ∨ r) ≡ (p ∧ q) ∨ (p ∧ r) |                   |
| p ∧ p ≡ p     | Idempotent Laws     | ¬(p ∧ q) ≡ ¬p ∨ ¬q              | De Morgan’s Laws  |
| p ∨ p ≡ p     |                     | ¬(p ∨ q) ≡ ¬p ∧ ¬q              |                   |
| ¬(¬p) ≡ p     | Double Negation Law | p ∨ (p ∧ q) ≡ p                 | Absorption Laws   |
| p ∨ q ≡ q ∨ p | Commutative Laws    | p ∧ (p ∨ q) ≡ p                 |                   |
| p ∧ q ≡ q ∧ p |                     | p ∨ ¬p ≡ T                      | Negation Laws     |
|               |                     | p ∧ ¬p ≡ F                      |                   |
