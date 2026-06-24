# SoC Generative Modeling & Diffusion — Midterm Submission

## Overview

This project is part of the Summer of Code (SoC) Generative Modeling and Diffusion track. The goal of the first half of the program has been to build a strong foundation in latent-variable generative models, beginning with the mathematical principles behind Variational Autoencoders (VAEs) and progressing toward training complete generative models on synthetic and image datasets.

The work completed so far covers:

1. VAE fundamentals and ELBO optimization
2. Training a Linear VAE on 2D synthetic data
3. Training a Convolutional VAE on the MNIST dataset
4. Latent space visualization, interpolation, and generation

---

## Week 2 — VAE Fundamentals

### Topics Covered

* KL Divergence between Gaussian distributions
* Reparameterization Trick
* Evidence Lower Bound (ELBO)
* Variational Inference Basics

### Implementations

* Closed-form KL divergence from scratch
* Reparameterization sampling
* ELBO loss implementation
* Analysis of latent-variable optimization

### Key Learning Outcomes

* Understood why direct maximization of log p(x) is intractable
* Learned how the encoder approximates the posterior distribution
* Implemented and verified the core mathematical components of a VAE

---

## Week 3 — Linear VAE on 2D Data

### Objective

Train a Variational Autoencoder on a synthetic 2D circles dataset and study latent-space behaviour.

### Implementations

* Linear encoder-decoder architecture
* Latent distribution parameterization (μ and log σ²)
* ELBO-based training
* Reconstruction and generation pipeline

### Visualizations

* Training loss curves
* Data reconstructions
* Latent-space embeddings
* Generated samples from the learned distribution

### Key Learning Outcomes

* Observed how latent representations emerge during training
* Studied the trade-off between reconstruction quality and KL regularization
* Investigated posterior collapse and the effect of β in β-VAEs

---

## Week 4 — Convolutional VAE on MNIST

### Objective

Extend the VAE architecture from vector inputs to image generation using convolutional neural networks.

### Architecture

* Convolutional Encoder
* Latent Space Representation
* Reparameterization Sampling
* Transposed-Convolution Decoder

### Dataset

MNIST Handwritten Digits Dataset

### Implementations

* Convolutional VAE
* BCE + KL ELBO objective
* Training and evaluation pipeline
* β-VAE experiments

### Visualizations

* Original vs Reconstructed Digits
* Randomly Generated Digits
* t-SNE Visualization of Latent Codes
* Latent Space Interpolation

### Experiments

Comparison of:

* β = 0.0
* β = 0.5
* β = 2.0

to study the impact of KL regularization on reconstruction quality and latent-space organization.


---


---

## Repository Structure

```text
.
├── Week2.ipynb
├── Week3.ipynb
├── Week4.ipynb
└── README.md
```

---


---



---

## Author

Rudra Bhor
B.Tech Mechanical Engineering
Indian Institute of Technology Bombay
