---
title: "Hensel's Proof of the Transcendence of e"
date: 2025-06-20
categories: [blog]
tags: [math, transcendence, p-adics, history]
layout: post
author_profile: true
---

In 1905, Hensel provided the following proof about the transcendence of $$e$$.  


![Hensel proof](https://nimath.github.io/images/hensel.png)


By the Taylor expansion of $$e^x$$ at $$0$$, and evaluating at $$x=p$$, we get:


$$e^p = \sum_{n=0}^{\infty} \frac{p^n}{n!} = 1 + p \sum_{n=1}^{\infty} \frac{p^{n-1}}{n!},$$

From this expansion, we see that $$e$$ satisfies an equation of the form $$y^p = 1 + pu$$, where $$u$$ is a $$p$$-adic unit (Exercise).

But the polynomial $$y^p - (1 + pu)$$ is irreducible over $$\mathbb{Q}_p$$, the fraction field of $$\mathbb{Z}_p$$:  
writing $$y = 1 + z$$ and expanding, we get

$$z^p + pz^{p-1} + \dots + pz - pu$$

which is irreducible by the **Eisenstein criterion**.  
Therefore $$e$$ must have degree at least $$p$$ over $$\mathbb{Q}_p$$. Hence:

$$[\mathbb{Q}(e) : \mathbb{Q}] \ge p,$$

but this is true for **any prime** $$p$$, so $$e$$ must be transcendental.

**Now, can you spot the flaw in this argument?** [If not, look for it on these  notes by K. Conrad](https://kconrad.math.uconn.edu/blurbs/gradnumthy/infseriespadic.pdf)

<small>The original reference is [here](https://www.digizeitschriften.de/id/37721857X_0014%7Clog145?tify=%7B%22pages%22%3A%5B554%2C555%5D%2C%22pan%22%3A%7B%22x%22%3A1.006%2C%22y%22%3A0.792%7D%2C%22view%22%3A%22toc%22%2C%22zoom%22%3A0.408%7D#navi)</small>

For a correct use of $$p$$-dic numbers in transcendence questions [check this out](https://mattbaker.blog/2015/03/20/a-p-adic-proof-that-pi-is-transcendental/) 
