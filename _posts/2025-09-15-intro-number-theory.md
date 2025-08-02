---
title: "An Introduction to Number Theory"
date: 2025-09-15
permalink: /posts/2025/09/intro-number-theory/
layout: single
author_profile: true
tags: [number theory, teaching]
---

*[Course presentation — Padova, September 2025](https://didattica.unipd.it/off/2025/LM/SC/SC2998/002PD/SCQ0094301/N0)*

---

## What is number theory?

In the third century, Diophantus of Alexandria investigated problems of the type:  
Given $$f \in \mathbb{Z}\left[X_1, ..., X_n\right]$$, can we find integer (or rational) solutions to:


$$f(X_1, ..., X_n) = 0 \quad ?$$

Number theory is broadly the study of this question and its generalizations, such as systems of polynomial equations.

### Examples

1. **Linear Diophantine equation:**

$$
aX_1 + bX_2 = m \quad \text{where } a, b, m \in \mathbb{Z}
$$

This is handled by the Euclidean algorithm.

2. **Fermat's equation:**

$$
X^n + Y^n = Z^n
$$

which has no non-trivial integer solutions for $$n > 2 $$. We will prove this when $$n $$ is a regular prime.

---

## A toy example

Consider:

$$
X^3 = Y^2 + 2
$$

Factoring over $$\mathbb{Z}\left[\sqrt{-2}
\right] $$:

$$
X^3 = (Y + \sqrt{-2})(Y - \sqrt{-2})
$$

Using:
- $$\mathbb{Z}\left[\sqrt{-2}\right] $$ is a UFD
- Its units are $$\pm1 $$
- $$Y + \sqrt{-2} $$ and $$Y - \sqrt{-2} $$ are coprime

We conclude the only solutions are $$(X, Y) = (3, \pm5) $$.

> Numbers like $$Y + \sqrt{-2}$$ were once called *ideal numbers* — inspiring the modern concept of ideals in rings.

---

## Conclusion

Solving equations like $$aX + bY = m $$ relies on unique factorization in $$ \mathbb{Z} $$. Similarly, solving $$X^3 = Y^2 + 2 $$ uses factorization in $$\mathbb{Z}\left\sqrt{-2}\right] $$. But in general, we must deal with rings that are not UFDs.

Hence, we develop the theory of **number fields**.

Let $$K $$ be a number field (a finite extension of $$\mathbb{Q} $$), and $$\mathcal{O}_K $$ its ring of integers. Then:

1. Every ideal $$I \subset \mathcal{O}_K $$ has a unique factorization:

$$
I = P_1^{e_1} \cdots P_n^{e_n}
$$

2. The unit group $$\mathcal{O}_K^\times $$ is a finitely generated abelian group with:

$$
\text{rank}(\mathcal{O}_K^\times) = r_1 + r_2 - 1
$$

where $$r_1 $$ = number of real embeddings, $$r_2 $$ = number of complex pairs.

3. The Dedekind zeta function $$\zeta_K(s) $$ satisfies:

$$
\lim_{s \to 1}(s - 1) \zeta_K(s) = \frac{2^{r_1}(2\pi)^{r_2} h_K R_K}{\omega_K \sqrt{|d_K|}}
$$
where all the main arithmetic invariants of the field $$K$$ show up.


During the course we will review all the basics of algebraic and analytic number theory, along with a lot of exercises and concrete examples.



