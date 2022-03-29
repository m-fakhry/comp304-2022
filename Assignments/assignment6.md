# Assignment 6

### 3/28/2022

---

Three different groups of assignments:
- **Lab** assignments are due on Wednesday April 6.
- **Paper** assignments are due on Monday April 11.
- **For your curiosity (FYC)** assignments are due on Monday April 4 and no need to submit them. Just keep it for your self.

---

1. Read sections 4.4.2, 4.4.3, 4.4.4


2. **(Lab)** Write an algorithm to compute the parsing table any any given LL(1) grammar. Hint: use the FIRST and FOLLOW sets algorithms.

3. **(Lab)** Write a table-driven parser for the problem in assignment 4. Hint: use the parsing table construction algorithm you wrote in exercise 2.

4. **(FYC)** Solve exercises 4.4.1, 4.4.3, 4.4.4 from the book.

5. **(FYC)** The following grammar is not suitable for a top-down predictive parser. Identify the problem and correct it by rewriting the grammar. Show that your new grammar satisfies the LL(1) condition(s).

        <L> -> <R>a | <Q>ba
        <R> -> aba | caba | <R>bc
        <Q> -> bbc | bc

6. **(Paper)** BONUS: Solve exercise 4.4.6
