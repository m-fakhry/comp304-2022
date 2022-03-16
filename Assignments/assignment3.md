# Assignment 3

### 3/7/2022

1. **(Paper)** Write a regular expression for the graph coloring language (in [Assignment 1](assignment1.md)).


2. **(Lab)** Write a C++ program that reads a file that has a string of the input language (graph coloring) and generates a stream of tokens. For example, converts the input file

 <pre><code data-trim data-noescape>
    (1,2),(1,red)
  </code></pre>

  &emsp;&emsp;&emsp;&emsp;to the token file

      < open_paranthesis, ( >
      < number, 1 >
      < comma, , >
      < number, 2 >
      < close_paranthesis, ) >
      < comma, , >
      < open_paranthesis, ( >
      < number, 1 >
      < comma, , >
      < color, red >
      < close_paranthesis, ) >
      < eof, >

&emsp;&emsp;&emsp; - Write a regular expression for the language and its DFA.

&emsp;&emsp;&emsp; - Implement the scanner in two different ways: table-driven and hand-coded.

&emsp;&emsp;&emsp; - Compare the two implementations in terms of running time and memory consumption.  
