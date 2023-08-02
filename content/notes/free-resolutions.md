+++
title="Free resolutions"
date=2020-03-26
+++

Homology and cohomomolgy of modules, which are $Ext$ ant $Tor$ in the universal coefficients theorem, are defined in terms of _free resolutions_. Here we define these and sketch the proofs of their existence and uniqueness.

Fix henceforth a ring $R$ and modules $M$ and $N$ over $R$. Note that $R$ may not be commutative, and we take $M$ and $N$ to be _bi-modules_.

#### Free resolutions

* A _free resolution_ of $M$ is an exact sequence `$\dots \to F_n \to \dots \to F_1 \to F_0 \to M \to 0$` such that each module `$F_k$` is free over $R$.
* The property of free modules we use is the following: suppose $F$ is free and `$A \overset{f}\to B \to 0$` is exact (i.e. $f$ is onto), and `$\varphi: F \to B$` is a morphism, then there exists a morphism `$\psi: F \to A$` such that `$\varphi = f \circ\psi$`.
* To show the above for a free module we just construct `$\psi$` on a basis. Modules satisfying the above are called _projective_, and in general are a larger class than free modules.
* The existence of free resolutions is elementary - we find `$F_0$` which surjects to $M$, then `$F_1$` which surjects to the kernel of the morphism `$F_0\to M$` etc.

#### Chain morphisms from morphisms

* Just as techniques in, for example, the theorem of Whitehead we saw let us first construct maps on spaces from those on fundamental groups, and then show two such maps are homotopic, here we extend morphisms of modules to morphisms of chain complexes, and also show these extensions are chain homotopic.
* First we sketch the construction of chain morphisms. Fix free resolutions `$F_* \to M$` and `$G_* \to N$` and a morphism `$\varphi: M\to N$`. We do not actually use that the second chain complex is free.
* First, note that by composition we get a morphism `$F_0\to M\to N$`. As `$G_0\to N\to 0$` is exact, we get a corresponding morphism `$F_0 \to G_0$`.
* We now proceed inductively. For example, we have a map by composition `$\theta: F_1\to G_0$`. Further we deduce from exactness that the image of `$\theta$` is in the kernel of `$G_0\to N$` and hence in the image of the morphism `$G_1 \to G_0$`. We can thus lift this to `$F_1 \to G_1$`.

#### Chain homotopies

* Suppose now we are given two chain morphisms `$\Phi$` and `$\Phi'$` extending `$\varphi: M\to N$`. We construct a chain homotopy $H$ between them, i.e., so that `$\partial H + H\partial = \Phi' - \Phi$`.
* We proceed inductively, and leave the base case for the induction as an exercise.
* Let us define `$H_n: F_n \to G_{n+1}$`. The condition to be satisfied by `$H_n$` is `$\partial\circ H_n = \Phi' - \Phi - H_{n-1}\circ \partial$`. This says that `$H_n$` is a _lift_ of the map `$\Theta:= \Phi' - \Phi - H_{n-1}\circ \partial\: F_n\to G_n$`.
* By freeness, the lift exists if (and only if) the image of `$\Theta$` is contained in the image of `$\partial: G_{n+1} \to G_n$`, which by exactness is the kernel of the next morphism.
* Thus, it suffices to show that for all `$\xi \in F_n$`, `$\partial(\Theta(\xi)) = 0$`.
* This can be deduced by the induction hypothesis, as `$\partial H(\partial \xi) + H(\partial \partial \xi) = \Phi'(\partial \xi) - \Phi(\partial\xi)$` and `$\partial\Theta(\xi) = \partial\Phi'(\xi) - \partial\Phi(\xi)-\partial H(\partial \xi) = \Phi'(\partial \xi) - \Phi(\partial\xi)-\partial H(\partial \xi)$`, with the second equality a consequence of `$\Phi$` and `$\Phi'$` being chain morphisms.

#### Uniqueness of resolutions

Given two free resolutions of $M$, we extend the identity morphism of $M$ to chain morphisms in both directions, and show that both compositions are chain homotopic to the respective identities.
