---
title: 'Serre-Tate for 1-motives'
date: 2017-06-22
permalink: /posts/2017/06/serre-tate/
tags:
  - math
---

This post is an overview of the article arXiv:1704.01340 written with A. Bertapelle. 

We generalise to 1-motives the classical correspondence  between the following sets
  - The set of deformations of an abelian variety $$A$$ in characteristic $$p>0$$;
  - The set of deformations of the Barsotti-Tate group of $$A$$.
  
A nice application is a concrete description of the formal moduli space of an ordinary abelian variety.

Deformation theory
------

Let $$X_0$$ be a smooth scheme over a field $$k$$ and let $$(R,\frak m)$$ be an Artin local ring with residue field $$k$$. Deformation theory is 
the study of schemes $$X/R$$ deforming $$X_0$$, i.e. $$X_k\cong X_0$$. Namely one looks for conditions under which such an $$X$$ exists and how many of them we can find.

Assume (for simplicity) that $$(\frak m)^2=(0)$$ (i.e. we just deal with first order infinitesimal deformations). The basic result of Grothendieck on deformation theory tells that

there exists an obstruction $$o(X_0)\in H^2(X_0,T_{X_0/k}\otimes \frak m)$$ such that $$o(X_0)=0$$ iff there exists $$X/R$$ deforming $$X_0$$.
if $$o(X_0)=0$$ the set of deformations corresponds to $$H^1(X_0,T_{X_0/k}\otimes \frak m)$$, and $$H^0(X_0,T_{X_0/k}\otimes \frak m)$$ corresponds to the group $$Aut(X/X_0)$$.
It follows quite easily that we can deform (at least formally) an abelian scheme $$A_0$$ as a scheme. Then because of properness and the existence of a zero section one can show that the group structure lifts too (with some work as explained in [4]).

Barsotti-Tate groups
------

The theory Barsotti-Tate groups (aka p-divisible groups) have many interesting applications like in Faltings' proof of Mordell-Weil or the Fontaine's results on the existence of abelian schemes over number rings. The motivating example is the following: let $$E/k$$ be an elliptic curve over some field. Then the scheme-theoretic kernel $$E(\ell^n)$$ of the multiplication 
by $$\ell^n$$ is a finite flat group scheme of rank $$2\cdot \ell^n$$. Now if $$\ell \ne char\ k$$ we an recover this group scheme by the associated galois module $$E(\ell^n)(k^{sep})\cong (\mathbb{Z}/\ell^n\mathbb{Z})^2$$. Whereas if $$\ell = p$$ is the characteristic of our base field $$E(\ell^n)(k^{sep})$$ is equal to $$\mathbb{Z}/\ell^n\mathbb{Z}$$ or $$0$$. 
This motivates the use of $$E(p^\infty)=\cup E(p^n)$$ which is the basic example of a Barsotti-Tate group.

For the record the fancy definition is a s follows ($$p$$ is fixed).  A BT group over $$S$$ (any base scheme) is an abelian fppf sheaf $$G$$ over $$S$$ such that

$$G$$ is p-divisible
$$G$$ is p-torsion
$$G[p]$$ is a finite flat group scheme
The main result

We fix $$k$$ of characteristic $$p>0$$ and we denote by $$Def(X_0/R)$$ the set of deformations of $$X_0$$ (a scheme, an abelian scheme or a BT group). Then Serre-Tate theory gives an isomorphism

$$ Def(A_0/R) \cong  Def (A_0 (p^\infty) / R)$$

for $$A_0$$ an abelian scheme over $$k$$. We proved the same statement (and more precisely a categorical equivalence) for $$A_0$$ replaced by a 1-motve $$M_0$$ over $$k$$.

As a consequence if $$M_0$$ is an ordinary 1-motive over an algebraically closed field we have the formula

$$ Def(A_0/R) = Hom (T_p M_0 (k) \otimes T_p {M_0}^* (k), \widehat{ \mathbb{G} }_m (R) )$$

and we can compute the Gauss-Manin connection of a deformation $$M/R$$.


About the proofs
------

I don't know the original proof given by Serre and Tate. In [1], which is the standard reference on the topic, is given the proof of Drinfel'd. Some part of it can be adapted to 1-motives, in particular for the fully faithfulness in weight $$\le 1$$. The difficult part of the proof is the essential surjectivity. For instance one cannot use the Grothendieck deformation theorem in order to lift a general 1-motives: already for a semi-abelian scheme there is something to do!

Certainly the key point is to understand what happen for the 1-motive $$[ \mathbb{Z}  \to \mathbb{G}_m ]$$. The BT group of such a 1-motive (say over $$\bar{\mathbb{F}}_p$$) is simply $$\mu_{p^\infty} \times \mathbb{Q}_p/\mathbb{Z}_p$$ (like for an ordinary elliptic curve). By Kummer theory (see [2]) one gets

$$Hom_R(\mathbb{Z}_p , \mu_{p^\infty}) \cong Ext^1_R( \mathbb{Q}_p/\mathbb{Z}_p, \mu_{p^\infty})$$ 

and I invite the interested reader to spend some time on this formula!

Further readings
------

I first learned about Serre-Tate theory by studying the personal notes of Olivier Brinon on BT groups. Then I went trough the classical references [1,2] with the help of [3,4,5].

[1] Katz: Serre-Tate local moduli

[2] Messing: Thesis, LNM 264

[3] Ward: blog posts ST1 and ST2

[4] Dospinescu: theorems of Serre-Tate and Grothendieck

[5] Amy (Cheung) Wooding: beamer on ST


[wordpress](https://nimazsite.wordpress.com/2017/06/22/serre-tate/)
