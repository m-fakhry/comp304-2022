# Lecture 5

## Top-Down Parser

- recursive descent parsing
  - can not handle left recursion
    - eliminating direct and indirect left recursion
  - can not handle common prefix
    - we might get an issue when defining lookahead so we need left factoring
    - left factoring A -> a B1 | a B2, which rule to use? A -> a A', A' -> B1 | B2
  - can not handle ambiguity
- First and Follow
  - algorithm for First and Follow
  - example

<!-- - LL1 (table-driven parser)
  - construction of parsing table
  - benefits of FIRST and FOLLOW sets -->
