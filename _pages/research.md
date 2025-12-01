---
layout: page
title: Research
permalink: /research/
nav: true
nav_order: 2
---

## Overview

<!-- TODO: Add graphical abstract/diagram here -->

**The Question:** How do biological circuits implement the computation required for flexible behavior?

My work combines mathematical theory, high-performance computing, and biological constraints to investigate the mechanistic basis of neural computation. I am specifically interested in how neural circuits infer and maintain latent representations of the environment to support zero-shot and few-shot learning.

## Core Themes

### 1. Neural Manifolds & Mechanistic Substrates

While the field often studies neural manifolds in abstract rate-based models, I aim to anchor these concepts in biological constraints.

* **Goal:** Develop a bridge between low-dimensional population dynamics and specific connectivity motifs in Spiking Neural Networks (SNNs).
* **Approach:** Using "in silico" models as testbeds to unify control theory, dynamical systems, and STDP-based learning rules.

### 2. Latent State Inference & Cognitive Flexibility

Animals can adapt to novel scenarios with minimal experience, suggesting they use "latent states" to represent context.

* **Hypothesis:** Circuits do not just overwrite synaptic weights during learning; they shift and modulate existing manifolds to represent new task rules.
* **Application:** Studying **Reversal Learning** and **Flexible Decision-Making** to understand how networks balance stability (remembering old tasks) with plasticity (learning new ones) without catastrophic interference.

## Toolbox

* **Theory:** Dynamical Systems, Graph Theory, Information Geometry.
* **Computation:** JAX/Flax for differentiable physics; CUDA for parallel acceleration.
* **Modeling:** Leaky Integrate-and-Fire (LIF) networks, Recurrent Neural Networks (RNNs), Evolutionary Optimization.
