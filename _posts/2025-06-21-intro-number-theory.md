---
title: "An Introduction to (Algebraic) Number Theory"
date: 2025-06-21
categories: [blog]
tags: [number theory, teaching, course]
layout: post
author_profile: true
---

*Course presentation — San Salvador, September 2016*

---

## What is number theory?

In the third century, Diophantus of Alexandria investigated problems of the type:  
Given \( f \in \mathbb{Z}[X_1, ..., X_n] \), can we find integer (or rational) solutions to:

\[
f(X_1, ..., X_n) = 0 \quad ?
\]

Number theory is broadly the study of this question and its generalizations, such as systems of polynomial equations.

### Examples

1. **Linear Diophantine equation:**

\[
aX_1 + bX_2 = m \quad \text{where } a, b, m \in \mathbb{Z}
\]

This is handled by the Euclidean algorithm.

2. **Fermat's equation:**

\[
X^n + Y^n = Z^n
\]

which has no non-trivial integer solutions for \( n > 2 \). We will prove this when \( n \) is a regular prime.

---

## A toy example

Consider:

\[
X^3 = Y^2 + 2
\]

Factoring over \( \mathbb{Z}[\sqrt{-2}] \):

\[
X^3 = (Y + \sqrt{-2})(Y - \sqrt{-2})
\]

Using:
- \( \mathbb{Z}[\sqrt{-2}] \) is a UFD
- Its units are \( \pm1 \)
- \( Y + \sqrt{-2} \) and \( Y - \sqrt{-2} \) are coprime

We conclude the only solutions are \( (X, Y) = (3, \pm5) \).

> These were once called *ideal numbers* — inspiring the modern concept of ideals in rings.

---

## Conclusion

Solving equations like \( aX + bY = m \) relies on unique factorization in \( \mathbb{Z} \). Similarly, solving \( X^3 = Y^2 + 2 \) uses factorization in \( \mathbb{Z}[\sqrt{-2}] \). But in general, we must deal with rings that are not UFDs.

Hence, we develop the theory of **number fields**.

Let \( K \) be a number field (a finite extension of \( \mathbb{Q} \)), and \( \mathcal{O}_K \) its ring of integers. Then:

1. Every ideal \( I \subset \mathcal{O}_K \) has a unique factorization:

\[
I = P_1^{e_1} \cdots P_n^{e_n}
\]

2. The unit group \( \mathcal{O}_K^\times \) is a finitely generated abelian group with:

\[
\text{rank}(\mathcal{O}_K^\times) = r_1 + r_2 - 1
\]

where \( r_1 \) = number of real embeddings, \( r_2 \) = number of complex pairs.

3. The Dedekind zeta function \( \zeta_K(s) \) satisfies:

\[
\lim_{s \to 1}(s - 1) \zeta_K(s) = \frac{2^{r_1}(2\pi)^{r_2} h_K R_K}{\omega_K \sqrt{|d_K|}}
\]

---

## Advanced Topics

**Class Field Theory** describes abelian extensions of local/global fields via arithmetic.  
We plan to outline core results and present the algebraic/cohomological approaches of Chevalley, Artin, and Tate.
