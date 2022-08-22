---
layout: post
title: Diffusion Models Beat GANs on Image Synthesis - A Summary
date: 2021-05-16 21:01:00
description: A summary of Diffusion Models Beat GANs on Image Synthesis.
tags: research notes-and-summaries
categories: Research
---

## Terminologies and Pre-requisite knowledge

* [Generative Adversarial Networks(GAN)](https://arxiv.org/abs/1406.2661)
* [Fréchet Inception Distance(FID)](https://en.wikipedia.org/wiki/Fr%C3%A9chet_inception_distance) - metric to assess the quality of images generated by a GAN. Unlike Inception Distance, it compares distribution of generated images with real images by training a standard network like Inception on real images and generated images and then comparing the Gaussian Distribution parameters of the deeper CNN layers
* Likelihood based Generative Models - class of generative models that model the distribution of data using a likelihood function. For instance, variational autoencoders.

## Introduction

* GANs capture less diversity than state-of-the-art likelihood-based models, are difficult to train, scale and apply to new domains.
* Likelihood based Generative Models capture more diversity, but are not able to produce high quality images.
* Diffusion models - a class of likelihood-based models, shown to produce high-quality images, while offering desirable properties such as distribution coverage, a stationary training objective, and easy scalability.
* **Hypothesis** -
    1. Model architectures used by recent GAN literature have been heavily explored and refined.
    2. GANs are able to trade off diversity for quality, producing high quality samples but not covering the whole distribution.
* **Aim** - In diffusion models, improve model architecture and then devise a scheme to trade off diversity for quality.

## Architecture improvements

* Existing architecture(Diffusion model) - [UNet Architecture](https://arxiv.org/abs/2006.11239)

## Paper and Code

* [Paper](https://arxiv.org/pdf/2105.05233v3.pdf)
* [Code](https://github.com/openai/guided-diffusion)