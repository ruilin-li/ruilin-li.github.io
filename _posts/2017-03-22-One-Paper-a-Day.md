---
layout: post
title: "One Paper a Day"
author: Ruilin Li
image: one-paper-a-day.jpg
meta: "Inspired by Neal Jean's post on Medium, I decide to start my 2017 challenge, reading at least one paper a day. Try to keep track of the latest progress in the area of machine learning."
---

Inspired by [Neal Jean's post](https://medium.com/@nealjean/2017-challenge-one-paper-a-day-9d7811accd09#.wqq4ozcim), I decide to start my 2017 challenge, reading at least one paper a day. Try to keep track of the latest progress in the area of machine learning.

* ### [Wasserstein GAN](https://arxiv.org/pdf/1701.07875.pdf)
Martin Arjovsky, Soumith Chintala, L´eon Bottou - **Mar 22, 2017**

_Wasserstein distance_ is  weaker than _Total Variance Distance (TV)_ and _Jenson-Shannon Divergence (JS)_. Moreover, all above three metric are weaker than _Kullback-Leibler Divergence (KL)_. A weaker distance metric induces a weaker topology in the space of all probability measures, a favorable setting for common gradient-based optimization algorithms, where convergence is easier in weak topology. The intractability of Wasserstein distance can be resolved by using _Kantorovich-Rubinstein duality_ and then we can optimize it over parameterized functions. Empirical results show that WGAN enjoys strong stability and is more robust to various network architechtures.


* 
