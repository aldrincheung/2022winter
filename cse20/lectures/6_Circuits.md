# Lecture 6: Circuits

#### Logical operators *aka propositional connectives*
|type|name|operator|latex|
|---|---|---|---|
|Conjunction|AND|$\land$|`\land`|
|Exclusive or|XOR|$\oplus$|`\oplus`|
|Disjunction|OR|$\lor$|`\lor`|
|Negation|NOT|$\lnot$|`\lnot`|

- *DNF* - disjunctive normal form - OR of ANDs of variables $(p \land a)\lor (p \land t) \lor (a \land t)$
- *CNF* - conjunctive normal form - OR of ANDs of variables $(\lnot p \lor \lnot a)\land (\lnot p \lor \lnot t) \land (\lnot a \lor \lnot t)$
  
|p|q|p $\to$ q|p $\leftrightarrow$ q|
|---|---|---|---|
|T|T|T|T|
|T|F|F|F|
|F|T|T|F|
|F|F|T|T|
| | |"if p then q"|"p if and only if q"|

#### Terms
|term|def.|
|---|---|
|Proposition|Declarative sentences that is true or false (not both). `this sentence is false` is **NOT** a proper proposition|
|Propositional variable|Variable that represents a propositon|
|Compound proposition|New proposition formed from existing propositions (*potentially*) using logical operators (propositional variable is considered to be a compound proposition)|
|Truth table|Table with one row for each of the possible combinations of truth values of the input & an additional column that shows the truth value of the result of the operation|
|Logical equivalence|Two compound propositions are logically equivalent means that thye have the same truth values for all settings of truth values to their propositional variables|
|Tautology|A compound proposition that evaluates to true for all settings of truth values to tis propositional variables; it is abbreviated T. `Ex.` $p \lor \lnot p$ **will always be true**
|Contradiction|A compound proposition that evaluates to false for all settings of truth values to its propositional variables; it is abbreviated F. `Ex.` $p \land \lnot p$ **will always be false**|
|Contingency|A compound proposition that is neither a tautology nor a contradiction|

#### More Terms
- The **hypothesis**/**antecedent** of $p \to q$ is $p$
- The **conclusion**/**consequent** of $p \to q$ is $q$
- The **converse** of $p \to q$ is $q \to p$
- The **inverse** of $p \to q$ is $\lnot p \to \lnot q$
- The **contrapositive** of $p \to q$ is $\lnot q \to \lnot p$ $\quad$ *is logically equivalent to p -> q* 


#### Equivalence "Theorems"
|name|of|
|---|---|
|Double negation|$\lnot(\lnot p)\equiv p$|
|**Commutativy** ordering of terms|$p\lor q\equiv q\lor p$ $\quad\quad$ $p\land q \equiv q \land p$|
|**Associativity** grouping of terms|$(p\lor q)\lor r \equiv p \lor(q\lor r)$ $\quad$ $(p\land q)\land r \equiv p \land(q\land r)$|
|**Domination** *aka short circuit evaluation*|$p\land F\equiv F$ $\quad$ $p\lor T\equiv T$ $\quad$ $p\land T\equiv p$ $\quad$ $p \lor F\equiv p$|
|**DeMorgan's Laws**|$\lnot(p \land q)\equiv \lnot p \lor \lnot q$ $\quad$ $\lnot(p \lor q)\equiv\lnot p \land\lnot q$|
|**Contrapositive**|$p\to q\equiv\lnot q\to\lnot p$|

Other equivalences
- $p\to q\equiv\lnot p\lor q$
- $\lnot(p\to q)\equiv p\land\lnot q$
- $\lnot(p \leftrightarrow q)\equiv p\oplus q$
- $(p\leftrightarrow q)\equiv q\leftrightarrow p$