---
title: "Around Fontaine’s Period Rings"
date: 2025-08-01
categories: [blog]
tags: [p‑adic Hodge, Fontaine, period rings, number theory]
layout: single
author_profile: true
---

> *Ich lebe mein Leben in wachsenden Ringen,  
> die sich über die Dinge ziehn.  
> Ich werde den letzten vielleicht nicht vollbringen,  
> aber versuchen will ich ihn.*  
>   
> *Ich kreise um Gott, um den uralten Turm,  
> und ich kreise jahrtausendelang;  
> und ich weiß noch nicht: bin ich ein Falke, ein Sturm  
> oder ein großer Gesang.*  
> — **Rainer Maria Rilke, 1899**

Rilke’s ever‑widening rings set the mood for these *informal notes on p‑adic period rings*: each new “ring” in Fontaine’s theory encircles the previous one, revealing deep arithmetic phenomena.  (I know this poem only thanks to Ignazio Longhi).
Below is a short summary of [a seminar I gave on this topic (PDF)](https://nimath.github.io/files/notes_on_fontaine_rings.pdf).

---

## A (really sketchy) timeline

| Year | Milestone |
|------|-----------|
| **1967** | Tate defines *p‑divisible groups* &nbsp;•&nbsp; Serre asks for their **periods** |
| **1979 – 1982** | Fontaine introduces *Barsotti–Tate rings* and constructs **$$B_{\mathrm{dR}}$$**, **$$B_{\mathrm{crys}}$$**, **$$B_{\mathrm{st}}$$** |
| **2011** | Beilinson re-proves the de Rham comparison in generality; Scholze coins the term *perfectoid* and open new ways|
| **since 2012** | Period rings (an their generalizations) drive modern p‑adic Hodge theory, Euler systems and beyond |



---

## Three important features 🍴

1. **The first ring already contains the period of the punctured disk.**  
   In the Fontaine construction one can consider  
   
     $$``2\pi i ''=t := \log\!\bigl([1^{\flat}]\bigr) = \sum_{n>0}\frac{(-1)^{n-1}\bigl([1^{\flat}]-1\bigr)^{n}}{n}$$
    
   and this mysterious element **generates the filtration** on $$B_{\mathrm{dR}}^{+}$$.

2. **Crystalline → semi‑stable → de Rham**  
   
     $$B_{\mathrm{crys}} \subset B_{\mathrm{st}} \subset B_{\mathrm{dR}}$$
    
   Every inclusion adds exactly the structure needed (Frobenius, then monodromy, then filtration) so that a Galois representation is *admissible* precisely when it comes from good, semi‑stable or general geometry.

3. **A single short exact sequence ties everything together.**  
   Fontaine’s *fundamental sequence*  
   
    $$\displaystyle 0\to Q_{p}(r)\to\mathrm{Fil}^{r}B_{crys}\xrightarrow{\varphi/p^{r-1}}B_{crys}\to 0$$

   giving the first link between étale and de Rham cohomology, the same way the integration of differential forms  over cycles realizes the connection between singular cohomology and and de Rham cohomology in the  classical setting.

---

* more details in the [PDF]((https://nimath.github.io/files/notes_on_fontaine_rings.pdf)) (comments are wellcome)

* An alternative to the poem is, [as suggested by Colmez](https://webusers.imj-prg.fr/~pierre.colmez/FW.pdf), the beggining of the lord of the rings. What is your choice?


