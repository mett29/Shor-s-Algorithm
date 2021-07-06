# Introduction

This project was done as part of the *Software Engineering 2* course at Polytechnic of Milan. The aim was to explore the field of Quantum Computing to understand its characteristics and potential. In order to accomplish this task, I and other colleagues started from the paper [Quantum Algorithm Implementations for Beginners](https://arxiv.org/pdf/1804.03719.pdf), from which each person chose an algorithm and then started its study. As you can understand, my algorithm is the Shor's algorithm.

# Shor's algorithm

Shor's algorithm, named after mathematician Peter Shor, is a quantum algorithm (an algorithm that runs on a quantum computer) for integer factorization, formulated in 1994. Informally, it solves the following problem: Given an integer **N**, find its prime factors.

## Disclaimer

GitHub has some issues in rendering LaTeX notation. Hopefully, everything should be understandable, otherwise use the following link to visualize the notebook:
- [Shor's algorithm (open with nbviewer)](https://nbviewer.jupyter.org/github/mett29/Shor-s-Algorithm/blob/master/Shor.ipynb?flush_cache=true)

Alternatively, just clone this repository and launch ```jupyter lab```.
```
git clone https://github.com/mett29/Shor-s-Algorithm.git
```

## Overview

*Lemma*: Factoring is equivalent to finding a nontrivial squareroot of 1 mod N.

**Complexity:**

- Complexity on quantum computer:
![quantum_complexity](https://wikimedia.org/api/rest_v1/media/math/render/svg/41344b55ef5e6494bb835b1adde9a4be4403303c)

- Complexity on classical computer:
![classical_complexity](https://wikimedia.org/api/rest_v1/media/math/render/svg/1956460a1cea4f2794fa0487f886e2a64cedc244)

<img src="img/complexity.png" width="650" height="300"/>

*Image credits: https://quantum-computing.ibm.com/docs/iqx/guide/shors-algorithm*

## Structure of the algorithm

Shor's algorithm consists of two parts:

**1) [CLASSICAL PART]** A reduction, which can be done on a classical computer, of the factoring problem to the problem of order-finding.

**2) [QUANTUM PART]** A quantum algorithm to solve the order-finding problem.

## References and resources

- [Wikipedia](https://en.wikipedia.org/wiki/Shor%27s_algorithm)
- [Original Shor's paper](https://arxiv.org/pdf/quant-ph/9508027.pdf)
- [Paper on QFT](https://courses.edx.org/c4x/BerkeleyX/CS191x/asset/chap5.pdf)
- [Paper on Modular Exponentiation](https://arxiv.org/pdf/quant-ph/0408006.pdf)
- [Beauregard's Circuit](https://arxiv.org/pdf/quant-ph/0205095.pdf)
- [Realization of a scalable Shor algorithm](http://science.sciencemag.org/content/351/6277/1068)
- [ProjectQ](https://projectq.readthedocs.io/en/latest/index.html)
- [Qiskit](https://qiskit.org/)
- [YouTube channel with explanation](https://www.youtube.com/channel/UCq9B8tT3oXl8BSyaoBPQXQw/videos?&ab_channel=PedroHenrique)
