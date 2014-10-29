## Notation

p(H) = Prior = probability of the hypothesis
p(D|H) = Likelihood = probability to see D if H is true
p(H|D) = Posterior = what we want to calculate (normally) = probability that the hypothesis is true with this data

P(H|D) = P(H)P(D|H)/P(D) -> P(D) can be the sum of P(D|H) for all hypothesis. This can be call the normalization, and it can be done if all the hypothesis are __mutually exclusive__ (at most one H in the set can be true) and __collectively exhaustive__ (at least one of the H has to be true)
