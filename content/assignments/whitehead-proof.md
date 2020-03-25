+++
title= "Proof of Whitehead's theorem"
date= 2020-04-02
+++

In this set of exercises, we complete some details of the proof of the theorem of Whitehead that was sketched as in the [worksheet](http://math.iisc.ac.in/~gadgil/algebraic-topology-2020/notebooks/Whitehead.ipynb.html). 

###### Part 1 - Existence of  maps

1. For the map `$f: X^{(1)} \to Y$` defined on the $1$-skeleton, show that `$f_* = \varphi\circ i_*$` where `$i: X^{(1)} \to X$ is the inclusion of the $1$-skeleton.
2. Conclude that of `$\theta: S^1 \to X^{(1)}$` is the attaching map of a $2$-cell in $X$, then `$f\circ\theta: S^1 \to Y$` is homtopically trivial.
3. Show that `$f: X^{(1)} \to Y$` extends to `$f: X^{(2)} \to Y$`, i.e., to a map on the $2$-skeleton.
4. Finally show that there exists `$f: (X, x_0)\to (Y, y_0)$` such that `$f_*=\varphi$`.

###### Part 2 - Homotopies of maps

Recall that we have a fixed maximal tree $T$ containing the base point `$x_0$`, and we define the homotopy $H$ on `$X^{(0)} \times [0, 1]$` as follows:
given a vertex $v$, there is a unique reduced path $\alpha$ in the tree $T$ from $x_0$ to $v$; map $v \times [0, 1]$ to $f_*(\bar\alpha) * g_*(\alpha)$.

1. Show that for an edge $e$ of $T$, the map $H$ defined as above extends to `$e\times [0, 1]$`.
2. Show that for an edge $e$ _not in_ $T$, the map $H$ defined as above extends to `$e\times [0, 1]$` (here we use `$f_* = g_*$`).
3. Show that $H$ extends to a homotopy from $f$ to $g$ on `$X\times [0, 1]$` (note that the this step involves only $n$-cells fof `$n\geq 3$`).
