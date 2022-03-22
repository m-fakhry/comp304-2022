# Lecture 4

## Scanner (Continue ...)

  - Hand-coded scanner
      - Memory efficient
  - Direct-coded scanner
      - Buffers

## Parser

  - Validates the string
  - Definition of CFG, derivation, leftmost/rightmost derivation, parse tree, ambiguity, priority

        <E> -> <E> + <T> | <E> - <T> | <T>
        <T> -> <T> * <F> | <T> / <F> | <F>
        <F> -> ( <E> ) | id
  - CFG vs RE (priority, ambiguity, etc.)
    - Example, if else statement
    - Example, multiplication and addition
  - **Classes of CFG (CFG, LR(1), LL(1), RE)**
  - Approaches for generating parser trees:
    - Top-down
      - **Recursive-Descent Parsing**


            void A() {
              Choose a production, <A> -> <X1><X2>...<Xk>
              for ( i = 1 to k ) {
                if ( Xi is a nonterminal )
                  call procedure Xi();
                else if ( Xi equals the current input symbol a )
                  advance the input to the next symbol;
                else /* an error has occurred */;
            }

      - algorithm, push the rule, match the word, or backtrack

      - eliminating (direct and **indirect**) left recursion

            <A> -> <A>a | b

            to

            <A>  -> b<A'>
            <A'> -> a<A'> | e
      - **backtrack-free parser**
        - lookahead: first set and follow set
        `FIRST(a)`, where `a` is any string of grammar symbols, to be the set of terminals that begin strings derived from `a`
        `FOLLOW(A)`, for nonterminal `A`, to be the set of terminals that can appear immediately to the right of `A` in some sentential (derivation) form
    - bottom-up
