# state-guide
overviews of consistency, availability and durability 

# levels

Level|Name|Phenomena disallowed
-----|----|-------
PL-CS|Cursor Stability|G1, G-cursor
PL-2L|Monotonic View|G1, G-monotonic
PL-MSR|Monotonic Snapshot Reads|G1, G-MSR
PL-2+|Consistent View|G1, G-single
PL-FCV|Forward Consistent View|G1, G-SIb
PL-SI|Snapshot Isolation|G1, G-SI
PL-2.99|Repeatable Reads|G1, G2-item
PL-3U|Update Serializability|G1, G-update
PL-3|Full Serializability|G1, G2

[source: Weak Consistency: A Generalized Theory and Optimistic
Implementations for Distributed Transactions](http://pmg.csail.mit.edu/papers/adya-phd.pdf)

# phenomena


Phenomenon|Description
----------|-----------
write cycles, G0|
aborted reads, G1a|
intermediate reads, G1b|
circular information flow, G1c|
non-atomic predicate-based reads, G1-predA|
non-atomic predicate-based reads w.r.t. transactions, G1-predB|
anti-dependency cycles, G2|
item anti-dependency cycles, G2-item|
non-atomic SQL statements, G-SQL-atomic|
anti-dependency cycles at runtime, E2|
single anti-dependency cycles, G-single|
monotonic reads, G-monotonic|
interference, G-SIa|
missed effects, G-SIb|
action interference, G-MSRa|
action missed effects, G-MSRb|
labeled single anti-dependency cycles, G-cursor(x)|
single anti-dependency cycles with update transactions, G-update|
single anti-dependency cycles at runtime, E-single|
monotonic reads at runtime, E-monotonic|
single anti-dependency cycles with update transactions at runtime, E-update|

[source: Weak Consistency: A Generalized Theory and Optimistic
Implementations for Distributed Transactions](http://pmg.csail.mit.edu/papers/adya-phd.pdf)


Phenomenon|Description
----------|-----------
dirty write, P0|
dirty read, P1|
cursor lost update|
lost update, P4|
non-repeatable/fuzzy read, P2|
phantom, P3|
read skew, A5A|
write skew, A5B|

[source: A Critique of ANSI SQL Isolation Levels](https://www.cs.umb.edu/cs734/CritiqueANSI_Iso.pdf)

Phenomenon|Description
----------|-----------
item-many-preceders, IMP|
predicate-many-preceders, PMP|
observed-transaction-vanishes, OTV|
non-monotonic reads, N-MR|
non-monotonic writes, N-MW|
missing read-write dependency, MRWD|
missing your writes, MYR|
lost update|
write skew|

[source: Highly Available Transactions: Virtues and Limitations
(Extended Version)](https://arxiv.org/pdf/1302.0309.pdf)
