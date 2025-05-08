---
layout: post
title: the Bellman equation for state values
date: 2022-12-12 15:30
description: a derivation
tags: probability reinforcement-learning
giscus_comments: true
related_posts: false
---

In their book "Reinforcement Learning: An Introduction", 2nd edition, 2018, Richard Sutton and Andrew Barto define the Bellman equation for state values in the following manner:

> $$
v_\pi(s) \doteq \mathbb{E}_\pi [G_t|S_t = s] = \sum_a \pi(a|s) \sum_{s^\prime} \sum_r p(s^\prime ,r|s,a) \Big[r + \gamma v_\pi(s^\prime)\Big] \qquad \forall \ s \in \mathcal{S}
$$

Seeing how it is that the right-hand side of this fascinating, recursive Bellman equation arises from the expectation expression on the left-hand side requires some understanding of probability theory. Sutton & Barto rightly focus on teaching reinforcement learning. Students of reinforcement learning are left to work out the probabilistic reasoning that gives rise to the Bellman equation for themselves.

Attached is a PDF containing a **derivation** of the Bellman equation for state values that takes readers from the expectation expression on the left-hand side to the fascinating, recursive expression on the right-hand side.  It was developed by me, for me, and for people like me --- people with only a basic grasp of probability theory who want a detailed, step-by-step derivation with lots of supporting explanation. Sophisticated probability people will likely find this derivation verbose and tedious.

<h1 class="post-title">
<a href="{{ 'Bellman_equation_derivation.pdf' | prepend: 'assets/pdf/' | relative_url}}" target="_blank" rel="noopener noreferrer" class="float-left"><i class="fas fa-file-pdf"></i></a>
</h1>

