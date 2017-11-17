---
layout: post
title: "One Paper a Day"
author: Ruilin Li
image: one-paper-a-day.jpg
markdown: kramdown
meta: "Inspired by Neal Jean's post on Medium, I decide to start my 2017 challenge, try to read one paper per day to keep track of the latest progress in the area of machine learning."
---

Inspired by [Neal Jean's post](https://medium.com/@nealjean/2017-challenge-one-paper-a-day-9d7811accd09#.wqq4ozcim), I decide to start my 2017 challenge, try to read one paper per day to keep track of the latest progress in the area of machine learning.

- ### [Algorithms for Inverse Reinforcement Learning](http://ai.stanford.edu/~ang/papers/icml00-irl.pdf)

  Andrew Y. Ng, Stuart Russell - Read on May 22, 2017

This paper did extensive experiments on sampling a representative sub-graph from a large graph. The authors proposed two types of goals - scale-down goal and back-in-time goal. The experiments showed that overall, random walk sampling and 'forest fire' sampling perform best, match most static and dynamic graph patterns well.



* ### [Sampling from Large Graphs](https://cs.stanford.edu/people/jure/pubs/sampling-kdd06.pdf)
  Jure Leskovic, Christos Faloutsos - Read on Mar 30, 2017

This paper did extensive experiments on sampling a representative sub-graph from a large graph. The authors proposed two types of goals - scale-down goal and back-in-time goal. The experiments showed that overall, random walk sampling and 'forest fire' sampling perform best, match most static and dynamic graph patterns well.


* ### [Automatic chemical design using a data-driven continuous representation of molecules](https://arxiv.org/pdf/1610.02415.pdf)
  Rafael Gomez-Bombarelli, David Duvenaud, Jose Miguel, Hernandez-Lobato, Jorge Aguilera-Iparraguirre, Timothy D. Hirzel, Ryan P. Adams, and Alan Aspuru-Guzik - Read on Mar 29, 2017

The idea of this paper is inspiring. Casting combinatoric object to an auto encoder, we can work with its latent, continuous, low dimensional(compared to original encoding) representation, where we have a great deal of powerful continuous optimization tools instead of local search for discrete structure. However, one difficulty needs to be addressed, once we have a latent representation, how we can make sure it is a valid one? What if it encodes to a non-exist combinatoric structure?



* ### [Towards Principled Methods for Training Generative Adversarial Networks](https://arxiv.org/pdf/1701.04862.pdf)
  Martin Arjovsky, Léon Bottou - Read on Mar 23, 2017

Even if the real data generating distribution $$P_{real}$$ and the fake generating distribution $$P_g$$ lie on two arbitrarily close manifolds, under mild conditions, $$ JS(P_{real} \| P_g) = \log 2 $$, meaning that essentially, this distance measure of two probability distributions is not 'continuous'. Moreover, the existence of optimal discriminator causes vanishing gradients on generator. When switching to $$ -\log D $$ alternative, the gradient has infinite variance, implying unstable training. The remedy could be either adding noise to discriminator or using softer distance measure such as _Wasserstein_.



* ### [Wasserstein GAN](https://arxiv.org/pdf/1701.07875.pdf)
  Martin Arjovsky, Soumith Chintala, L´eon Bottou - Read on Mar 22, 2017

_Wasserstein distance_ is  weaker than _Total Variance Distance (TV)_ and _Jenson-Shannon Divergence (JS)_. Moreover, all above three metric are weaker than _Kullback-Leibler Divergence (KL)_. A weaker distance metric induces a weaker topology in the space of all probability measures, a favorable setting for common gradient-based optimization algorithms, where convergence is easier in weak topology. The intractability of Wasserstein distance can be resolved by using _Kantorovich-Rubinstein duality_ and then we can optimize it over parameterized functions. Empirical results show that WGAN enjoys strong stability and is more robust to various network architectures.



* ### [Generative Adversarial Nets](https://arxiv.org/pdf/1406.2661.pdf)
  Ian J. Goodfellow, Jean Pouget-Abadie, Mehdi Mirza, Bing Xu, David Warde-Farley, Sherjil Ozair†, Aaron Courville, Yoshua Bengio - Read on Mar 21, 2017

_GAN_ combines generative model and discriminative model, simultaneously training two neural networks to learn the generating probability of the data. The value function to maximize here is

$$
	\displaystyle \min_{G}\max_{D} V(D,G) = \mathbb{E}_{\boldsymbol{x} \sim p_{data}(\boldsymbol{x})} [\log D(\boldsymbol{x})] - \mathbb{E}_{\boldsymbol{x} \sim p_{x}(\boldsymbol{x})} [\log D(\boldsymbol{x})]    
$$

and the paper showed convergence of the algorithm under reasonable condition. Actually, this creative framework can be extended to train various generative models.
