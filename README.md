# state-guide
overviews of consistency, availability and durability 


Level|Name|Phenomena disallowed
----------------
PL-CS|Cursor Stability|G1, G-cursor
PL-2L|Monotonic View|G1, G-monotonic
PL-MSR|Monotonic Snapshot Reads|G1, G-MSR
PL-2+|Consistent View|G1, G-single
PL-FCV|Forward Consistent View|G1, G-SIb
PL-SI|Snapshot Isolation|G1, G-SI
PL-2.99|Repeatable Reads|G1, G2-item
PL-3U|Update Serializability|G1, G-update
PL-3|Full Serializability|G1, G2


[source](http://pmg.csail.mit.edu/papers/adya-phd.pdf)

# phenomena
write cycles
aborted reads
intermediate reads
circular information flow
observed transaction vanishes
predicate-many-preceders
lost update
read skew
write skew
anti-dependency cycles

## ansii
p0
p1
p2
p3

dirty write
dirty read
fuzzy/non-repeatable read
phantom read

