---
layout: post
title: Transformers and HPC
date: 2022-09-12 03:24:42 +0100
mathjax: true
---

<details>
fdasf asd

  <summary>
  </summary>

- [1. Background on Transformers](#1-background-on-transformers)
  - [1.1. Transformers vs. RNN's (Motivation 1)](#11-transformers-vs-rnns-motivation-1)
  - [1.2. Useful info](#12-useful-info)
    - [1.2.1. Softmax](#121-softmax)
- [2. Workflow for AAYN model](#2-workflow-for-aayn-model)
- [3. Transformer architectures](#3-transformer-architectures)
- [4. Comments](#4-comments)

</details>

# 1. Background on Transformers

## 1.1. Transformers vs. RNN's (Motivation 1)

**Idea:** Framing transformers as an alternative to RNN’s for “sequence-to-sequence” mapping, e.g., for translation

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

## 1.2. Useful info

### 1.2.1. Softmax

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

# 2. Workflow for AAYN model

1. Inputs come in as a sequence of tokensfdas
2. fda

# 3. Transformer architectures

References:

What defines a transformer? What are its important properties, how does it differ from other kinds of architectures (and what are the current views of the effects of these differences?)

# 4. Comments

| Comments: |
| --------- |


| Is there any interesting way to relate some of these transformer vs RNN ideas to the distinc
