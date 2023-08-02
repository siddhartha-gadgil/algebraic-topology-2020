+++
title= "Spaces and Questions"
date= 2020-03-22
+++

__Note:__ The title alludes to a paper of Gromov, but needless to say this note is much more prosaic.

The goal of _Algebraic Topology_ is to answer questions about spaces - obviously including _topological_ questions but sometimes indirectly other questions as well. We have already seen many results that can help us answer these - _invariance of dimension_, the _Jordan-Brouwer separation theorem_, the _fixed point theorems_ of Brouwer and Lefschetz etc. Here we discuss a sample of questions that we can answer by the end of the course, or perhaps with a little more mathematics of the same nature.

##### Friends of Jordan-Brouwer

Let `$\Sigma$` be a compact, _orientable_ surface without boundary (for example a torus).

__Question:__  Does every embedding `$f: \Sigma\to S^3$` separate `$S^3$` into two components?

Next, let `$\Sigma$` be a compact, _non-orientable_ surface without boundary (for example `$\mathbb{R}P^2$`).

__Question:__ Is there an embedding of `$\Sigma$` in `$S^3$`?

##### Maps of Projective spaces

__Question:__ Is there a function `$f: \mathbb{C}P^2\to \mathbb{C}P^2$` that has no fixed point?

First, let us see if we can answer this question with the technology we have.

1. By using cellular homology, we know that `$H_k(\mathbb{C}P^2)$` is `$\mathbb{Z}$` for `$k = 0,2,4$` and `$0$` in all other cases.
2. By the Lefschetz fixed  point theorem, we have a fixed point unless the Lefschetz index satisfies `$\tau(f)=0$`.
3. The Leschetz index is the sum `$d_0 + d_2 + d_4$` of three "degrees" (using the obvious notion of the degree of an automorphism of `$\mathbb{Z}$`).
4. Further `$d_0 = 1$`.

Observe that this is not enough to show there is a fixed-point - we could have `$d_2 = -2$` and `$d_4 = 1$` for example. However we will see more, namely `$d_4 = d_2^2$`.  This implies that we must have a fixed point. Indeed, the same techniques let us answer the following classical question.

__Question:__ For what $n, m\geq 0$ do we have an _odd_ map `$f: S^n \to S^m$`?

##### Bounding surfaces

The solid torus $M = D^2 \times S^1$ has boundary $T = S^1 \times S^1$. But can we do "better"?

__Question:__ Is there a compact, _contractible_, (orientable) three-dimensional manifold $M$ with `$\partial M = T$`?

##### Homotopy type and the fundamental group

From the classification of surfaces, it is easy to deduce that for two compact, connected surfaces without boundary, being homotopy equivalent is equivalent to having isomorphic fundamental groups, as both these are equivalent to being homeomorphic. On the other hand, for dimensions above $3$, this is clearly false as, for example, $S^4$ and `$\mathbb{C}P^2$` are both simply-connected but are not homotopy equivalent. 

In dimension three, however, we have the following non-trivial questions. Note that we can ask the same questions with _homotopy equivalent_ replaced by _homeomorphic_, but for answering these (at least positively) we will have to use some form of Geometric Topology.

__Question:__ Is every simply-connected, compact, $3$-dimensional manifold without boundary _homotopy equivalent_ to $S^3$?

Here are two variants.

__Question:__ Are all pairs `$M_1$`, `$M_2$` of compact, connected $3$-dimensional manifolds with `$\pi_1(M_1) = \pi_1(M_2)$` homotopy equivalent?

__Question:__ Is every compact, $3$-dimensional manifold without boundary $M$ with `$\pi_1(M)\cong \mathbb{Z}^3$` _homotopy equivalent_ to $S^1\times S^1\times S^1$?

##### Answering the questions

Most of the above questions can be answered with the material of the rest of the course: Whitehead theory, cohomology, cup and cap products and Poincare duality. A couple need a 
little more - _Alexander duality_ and _ends of groups_, which if they are not covered in the course can be read up easily. Observe that the above _questions_ involve either no algebraic topology or only the fundamental group.
