[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/AtNXzL3S)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

-Based on work from last semester

According to the definition every pair of nodes that have an edge between them in $G_1$ should
be able to be transformed by the bijection to an equivalent in $G_2$, $(u,v)
\in E_1$ if $(f(u),f(v)) \in E_2$, therefore if the graphs dont have the same amount of nodes then there could be
a case where the graph $G_1$ has an edge between two nodes but graph $G_2$ does not have one of those nodes
leaving it wihout an equivalent edge, which would make $(u,v)
\in E_1$ if $(f(u),f(v)) \in E_2$ False.

An example would be:

Graph A: 

    {'a': {'b': 7, 'c': 4},

    'b': {'c': 3},

    'c': {}}

$V_1$ = (a,b,c)

Edges of A: $E_1$ = (a,b) (a,c) (b,c)

Graph B: 

    {'w': {'x': 7},

    'x': {}}


$V_2$ = (w,x)

Edges of B: $E_2$ = (w,x)

 f(a) -> w

 f(b) -> x

 f(c) -> does not have an equivalent

 meaning that (a,c) (b,c) which are $\in E_1$ do not have an equivalent of (f(a),f(c)) and (f(b),f(c)) $\in E_2$

 