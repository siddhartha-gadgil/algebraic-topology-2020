+++
title="Poincare duality"
date=2020-03-31
+++

#### Cup products: relative,  manifolds with boundary

* Relative cochains \(C^*(X, A)\) are cochains that _vanish_ on $A$.
* For manifolds with boundary, there is no co-cycle condition at the boundary, so co-chains are _similar to_ properly embedded submanifolds with boundary.
* On the other hand, _relative_ co-cycles correspond to closed manifolds.

#### Geometry of Poincar&eacute; duality

* Given a cell decomposition of an oriented $n$-dimensional manifold $M$, we can construct a _dual_ cell decomposition.
* The cellular chain complex for the dual cell decomposition is the cellular cochain complex of the original cell decomposition.
* Hence we get \[H^k(M) = H_{n- k}(M)\]
* For manifolds with boundary, we have corresponding statements:
\[H^k(M, \partial M) = H_{n- k}(M) \]
\[H^k(M) = H_{n- k}(M, \partial M) \]

#### Local homology, _restricting_ homology

* Fix a space $M$.
* The local homology at a point is \(H_*(M, M\{x\})\).
* By excision, \(H_*(M, M\setminus\{x\}) = H_*(U, U\setminus\{x\})\) if $U$ is open and \(x \in U\).
* In particular if $M$ is a manifold we know the local homology.
* More generally, for \(A \subset M\) we define \(H_*(M\vert A) = H_*(M, M\setminus A). \)
* This is _contravariant_ in $A$, with restriction; similarly cohomology restricted to $A$ is _covariant_.

#### Cohomology with compact support

* Assume $M$ has an exhaustion by compact sets (true for manifolds).
* Define \(H^*_c(M) = \lim H^*(M, M\ K)\) with respect to the ordering by compact sets.
* In the case where $M$ is compact, this is just the ordinary cohomology, but not for $\mathbb{R}$.

#### Orientations and the Fundamental class

* Let $M$ be a connected $n$-dimensional manifold.
* For a ring $R$ we define the orientation cover.
* We consider the rings \(\mathbb{Z}\) and \(\mathbb{Z}/2\).
* A local orientation is a choice of generator \(\mu_x\in H_*(M\vert x)\) for each \(x\in M\), which is locally constant:
* We say $M$ is _oriented_ if $M$ has a local orientation at each point.
* __Theorem:__ If $M$ is closed and oriented, then \(H_n(M; R)= R\) and \(H_k(M, R) = 0\) for $k > n$.
* We work inductively, so we want a statement for non-compact manifolds.
* __Lemma:__ Let $M$ be a connected $n$-dimensional manifold and $A\subset M$ be compact.
    * (a) \(H_i(M\vert A; R) = 0\) if $i > n$ and a class $z\in H_n(M, A; R)$ is zero if and only if its image is zero in each \(H_n(M\vert x; R)\).
    * (b) Given a local orientation \(\mu_x\) there is a class \(\mu\in H_n(M; R)\) that restricts to \(\mu_x\) for all \(x\in A\).
* We work inductively, using
\[0 \to H_n(M\vert A\cup B)\to H_N(M\vert A)\oplus H_n(M\vert B)\to H_n(M\vert A\cap B)\]
* The generator \(\mu\in H_n(M; R)\) we obtain in the compact case is called the _fundamental class_.

#### Cap product

* \(\cap: C_k(X; R) \times C^l(X; R)\to C_{k-l}(X; R)\) is given by 
\[\sigma\cap \varphi = \varphi(\sigma\vert_{<v_0, \dots, v_l>})\sigma\vert_{<v_l, \dots, v_k>}\]
* We have \(\partial \sigma\cap\varphi = (-1)^l(\partial \sigma\cap \varphi - \sigma\cap\delta\varphi)\), hence induces pairing on homology and cohomology.
* In fact, we get
\[H_k(X, A;R)\times H^l(X; R)\to H_{k -l}(X, A; R),\\
H_k(X, A;R)\times H^l(X, A; R)\to H_{k -l}(X; R).\]
* Further, \(\psi(\sigma\cap \varphi)= (\psi\cup\varphi)(\sigma)\).

#### Poincar&eacute; duality

* The statement o Poincar&eacute; duality is in fact that the cap product with the fundamental class is an isomorphism.
* For (in general) non-compact, $R$-oriented manifold, let \(D_M: H_c^k(M; R)\to H_{n- k}(M; R)\) be the limit of cap products with fundamental class.
* We see \[D_M: H_c^k(M; R) \overset{\cong}\to H_{n- k}(M; R).\]
* This follows inductively.
