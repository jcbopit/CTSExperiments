# Constant Term Sequence Experiments

This repository contains code developed by Justin Offutt for conducting computational experiments related to constant term sequences of Laurent polynomials modulo small primes. The work builds on and utilizes the SageMath library developed by Nadav Kohen: [`nkohen/ConstantTermSequences`](https://github.com/nkohen/ConstantTermSequences).

## 📚 Project Overview

The experiments in this repo were used in the paper:

> **Counterexamples to a Conjectured Bound on Constant Term Sequences Modulo Primes**  
> *Justin Offutt, Indiana University*

The goal was to test a conjectured upper bound on the location of the first zero in constant term sequences modulo a prime \( p \). Specifically, the conjecture suggested that for a fixed polynomial \( P(x) \), the first \( n \) such that
\[
\text{ct}[P^n(x)] \equiv 0 \pmod{p}
\]
would always satisfy \( n < p^{\deg P(x)} \). This repo contains randomized search code that discovered explicit counterexamples to this bound for degree-2 polynomials.

## 🧰 Dependencies

- **SageMath** (must be used as the Jupyter kernel)
- **SymPy**
- **NumPy**
- **Jupyter Notebook**

You also need to clone and include Nadav Kohen’s SageMath library:

```bash
git clone https://github.com/nkohen/ConstantTermSequences.git

```

The main experiments are in a jupyter notebook called "experiments".
You must run this notebook using the SageMath Jupyter kernel. If you have SageMath installed, you can launch the notebook interface using:

```bash
sage -n jupyter
```
