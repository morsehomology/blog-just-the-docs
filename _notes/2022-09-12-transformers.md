---
layout: post
title: Transformers and HPC
date: 2022-09-12 03:24:42 +0100
mathjax: true
---

<div class="t">Transformers and HPC</div>

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}

</details>

<details>
  <summary>
  </summary>

- [1. Presentation Outline](#1-presentation-outline)
  - [1.1. Background on Transformers](#11-background-on-transformers)
    - [1.1.1. Framing transformers as an alternative to RNN’s for “sequence-to-sequence” mapping, e.g., for translation (Idea 1)](#111-framing-transformers-as-an-alternative-to-rnns-for-sequence-to-sequence-mapping-eg-for-translation-idea-1)
    - [1.1.2. Useful info](#112-useful-info)
      - [1.1.2.1. Softmax](#1121-softmax)
  - [1.2. Workflow for AAYN model](#12-workflow-for-aayn-model)
  - [1.3. Transformer architectures](#13-transformer-architectures)
  - [1.4. Comments](#14-comments)

</details>

# 1. Presentation Outline

## 1.1. Background on Transformers

### 1.1.1. Framing transformers as an alternative to RNN’s for “sequence-to-sequence” mapping, e.g., for translation (Idea 1)

Here, each network will represent a function $f: X \to X'$, where $X$ and $X'$ denote the spaces of input and output sequences, respectively.

More specifically, let $T, T'$ denote the spaces of input and output tokens, and let $I$ denote the index set (need to elaborate on the structure of $I$). Then

$$
X = \{I \to T\}
$$

and

$$
X' = \{I \to T'\}
$$

Let $M = \{X \to X'\}$ denote the space of all sequence-to-sequence mappings.

### 1.1.2. Useful info

#### 1.1.2.1. Softmax

Softmax function $\rho: \R^n \to \R^n$,

$$
\rho\left(x_i\right)=\frac{\exp \left(x_i\right)}{\sum_j \exp \left(x_j\right)}
$$

Possible ways to think about it:

- Define $\rho_t$ by

$$
\rho_t\left(x_i\right)=\frac{\exp \left(t x_i\right)}{\sum_j \exp \left(t x_j\right)}
$$

for $t\in \R^+$.

## 1.2. Workflow for AAYN model

1. Inputs come in as a sequence of tokens
2.

## 1.3. Transformer architectures

References:

What defines a transformer? What are its important properties, how does it differ from other kinds of architectures (and what are the current views of the effects of these differences?)

## 1.4. Comments

| Comments: |
| --------- |


| Is there any interesting way to relate some of these transformer vs RNN ideas to the distinc
