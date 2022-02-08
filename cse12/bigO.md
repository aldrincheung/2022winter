# O notation

Big O notation describes the running time function of an algorithm w/ rules of:
1. If $f(N)$ is a sum of several terms, the highest order term (fastest growth rate) is kept and others are discarded
2. If $f(N)$ has a term that is a product of several factors, all constants are ommited

|Notation|Name|`Ex.`|
|---|---|---|
|$O(1)$|Constant|No loops nor recursive components|
|$O(\log N)$|Logarithmic|Get rids of a portion to be processed each time|
|$O(N)$|Linear|Loops once|
|$O(N\log N)$|Linearithmic|