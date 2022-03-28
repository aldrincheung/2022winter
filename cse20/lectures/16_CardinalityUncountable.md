# Lecture 16: Uncountably Infinity

### Cardinality categories
|category|def.|
|---|---|
|finite|the set is sempty or it is the same size as ${1,\cdots ,n}$ for some $n\in \mathbb{Z}^+$|
|countably infinite|the set is the same size as $\mathbb{N}$ (all countably infinite sets - same size)|
|countable|the set is either finite or countably infinite|
|uncountable|the set is not countable|

<br/>

### Lemmas about countable and uncountable sets & mod
|#|Lemma|
|---|---|
|0|if A $\leq$ B then $|A|\leq |B|$|
|1|If A is a subset of a countable set, then A is countable|
|2|If an uncountable set is a subset of A, then A is uncountable|
|3|If A and B are countable sets, then $A\cup B$ is countable and $A\cap B$ is countable|
|4|If A and B are countble sets, then $A\times B$ is countable|
|5|If A is a subset of B, to show that $|A|=|B|$ it's enuogh to give one-to-one function from A to B or an onto function from A to B|
|1|For $a,b\in\mathbb{Z}$ and positive integer $n$, $(a,b)\in R_{mod n}$ if and only if $n|a-b$|

<br/>


### Properties of a relation
|property|what it is|in english|
|---|---|---|
|reflexive|every element is related to itself<br/>$\forall a\in A(~(a,a)~\in R)$|every element is related to itself|
|symmetric|$\forall a\forall b(~(a,b) \in R \to (b,a) \in R ~)$|order doesn't matter for this relation|
|transitive|$\forall a\forall b\forall c(~((a,b)\in R \land (b,c)\in R)~\to~(a,c)\in R)$|chains of relations collapse|
|antisymmetric|$\forall a\forall b(~((a,b)\in R\land (b,a)\in R)\to a=b~)$|the relation has directionality|
|equivalence relation|the set is **reflexive**, **symmetric**, and **transitive**|
|partial ordering|the set is **reflexive**, **antisymmetric**, and **transitive**|

<br/>

### Axioms for Real Numbers (Order axioms)
|axiom|def.|
|---|---|
|Reflexitivity|Any number is less than or equal to itself<br/>$\forall a\in\mathbb{R}(a\leq a)$|
|Antisymmetry|If any two number are less than each other than they are equal<br/>$\forall a\in\mathbb{R}\forall b\in\mathbb{R}(~(a\leq b\land b\leq a)\to(a=b)~)$
|Transitivity|$\forall a\in\mathbb{R}\forall b\in\mathbb{R}\forall c\in\mathbb{R}(~(a\leq b\land b\leq c)\to (a\leq c)~)$|
|Trichotomy|All two numbers must either be equal to less than or more than<br/>$\forall a\in\mathbb{R}\forall b\in\mathbb{R}(~(a=b\lor b>a\lor a<b)~)$|

<br/>

### Uncountable Diagonal Proof
- relies on the set $D_f$

<br/>

### General Facts
- For two sets A, B, we use the nation $|A|<|B|$ to denote $(|A|\leq |B|)\land\lnot (|A|=|B|)$

<br/>

### Others
- $\mathbb{Q}$ (countably infinite) and $\mathbb{R}$ (uncountable) both have:
  - no greatest element
  - no least element
  - is true for $\forall x\forall y(x<y\to\exists z(x<z<y))$
- Least upper bound: Every nonempty set of real numbers that is bouncded above has a lesat upper bound
- Nested intervals: For each sequence of intervals $[a_n, b_n]$ where, for each $n$, $a_n<a_{n+1}<b_{n+1}<b_n$, there is at least one real number $x$ such that, for all $n$, $a_n\leq x\leq b_n$