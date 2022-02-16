# Lecture 9: Proofs

### Proof Wording
- Consider ..., an **arbitrary** ... **Assume** ..., we **want to show** that ... Which is what was needed, so the proof is complete.

### Proofs
|type|to proof|how.|name|
|---|---|---|---|
|predicate|$\forall xP(x)$ <br/>or<br/>$\lnot\exists xP(x)$|<br/>To prove when $P$ has finite domain, evaluate the predicate at **each** domain element<br/><br/>**Toward** a proof by univeral generalization, Let $e$ be an arbitrary element of $\mathbb{N}$<br/>**By** definition of $\mathbb{N}$, since $e\in\mathbb{N}$, (more info by deducing from $e$...). (relate it to the question).<br/>**This** is what was required.<br/>&nbsp;|Proof of universal by exhaustion|
|predicate|$\forall xP(x)$ <br/>or<br/>$\lnot\exists xP(x)$|<br/>To prove that $P$ with infinite domain, we take an **arbitrary** element $e$ from the domain of quantification and show that $P(e)$, without making any assumptions about $e$ other than that it comes from the domain.<br/><br/>**Toward** ...<br/>**case 1** $e=$:<br/>...<br/>&nbsp;|Proof by universal generalization|
|cond.|$p\leftrightarrow q$|<br/>**Toward** ...<br/>Goal 1: $p\to q$: ...<br/>Goal 2: $q\to p$: ...<br/>&nbsp;|~ exhaustion|
|cond.|$p\to q$|<br/>assume $p$ is true and ues that assumption to show $q$ is true<br/>&nbsp;|proof of conditional by direct proof|
|cond.|$p\to q$|<br/>assume $q$ is false and use that assumption to show $p$ is also false<br/>&nbsp;|proof of conditional by contrapositive proof|
|rewrite|$p\lor q$|<br/>rewrite it as equal to $\lnot p\to q$, and proof that<br/>&nbsp;|proof of disjunction using equivalent conditional|
|cases|$q$|<br/>**all possible** cases, $p_1,\ p_2,\ \cdots$<br/>case 1: show that $p_1\to q$ ...<br/>case 2: show that $p_2\to q$ ...<br/>we can conclude that $q$ is true<br/>&nbsp;|proof by cases|
|conj.|$p\land q$|<br/>proof $p$ is true<br/>proof $q$ is true<br/>&nbsp;|proof of conjunctions with subgoals|
|disproof|$\lnot\forall$|<br/>use counterexample<br/>&nbsp;||
|Predicate|$\exists xP(x)$|<br/>use witness<br/>&nbsp;||
|contradict|$p$|<br/>pick another statement $r$ and once we show that $\lnot p\to (r\land\lnot r)$, we can conclude that p is true<br/>&nbsp;|Proof by Contradiction|

<br/>

### Terms
|term|def.|
|---|---|
|counterexample|<br/>an element of which $P(X) = F$ within/of $\forall x\ P(x)$<br/>&nbsp;|
|witness|<br/>an element of which $P(X) = T$ within/of $\exists x\ P(x)$<br/>&nbsp;|
|Cartesian product| $A \times B = \{ (a, b) \|\ a\in A\land b\in B \}$|
|Union|All of the two sets: $A\cup B=\{x\|x\in A\lor x\in B\}$|
|Intersection|Elements that are in both sets: $A \cap B=\{x\|x\in A\land x\in B\}$|
|Set difference|A minus anything in set B (w/out intersection): $A-B=\{x\|x\in A\land x\notin B\}$|
|Disjoint sets|None of A is in B, vise versa: $A\cap B=\emptyset$|
|Power set|When $U$ is a set, $\mathcal{P}(U)=\{X\|X\subset U\}$|

<br/>

### Types of proofs
|type|what it is|
|---|---|
|Proof of universal by exhaustion|To prove that $\forall xP(x)$ is true when $P$ has a finite domani, evaluate the predicate at each domain element to confirm that it is always T|
|Proof by universal generalization|To prove that $\forall xP(x)$ is true, we can take an arbitarary element $e$ from the domain of quantification and show that $P(e)$ is true, without maing any assumption about e other than that it comes from the domain<br/>An **arbitrary** element of a set or domain is a fixed but known element from that list<br/><br/>"Let $e$ be an arbitrary element of N"|
