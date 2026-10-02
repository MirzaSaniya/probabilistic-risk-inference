# Probabilistic Risk Inference Engine

A lightweight Bayesian-network project for reasoning under uncertainty. The example models operational risk from observable evidence such as elevated load, anomaly signals, and service symptoms.

## Why this project matters

Many real decisions cannot be made from deterministic rules. Bayesian inference lets a system update beliefs as new evidence arrives and quantify uncertainty instead of returning only a hard label.

## Model

Example variables:

- `HighLoad`
- `Anomaly`
- `Failure`

The network encodes prior probabilities and conditional probabilities. The inference function computes posterior risk such as `P(Failure=True | evidence)` by enumeration.

## Run

```bash
python examples/demo.py
```

## Tests

```bash
pytest -q
```

## Portfolio talking points

- difference between priors, likelihoods, and posterior beliefs
- why correlated evidence needs careful modeling
- how posterior probability changes as evidence accumulates
- limitations of manually specified probabilities

## CS221 connection

Inspired by probabilistic inference and Bayesian-network concepts commonly covered in CS221. The example application and implementation are independently developed.

## GitHub metadata

**Repository name:** `probabilistic-risk-inference`

**Description:** A Bayesian network for reasoning under uncertainty and estimating risk from observed evidence.

**Topics:** `artificial-intelligence` `bayesian-networks` `probabilistic-inference` `probability` `uncertainty` `python` `machine-learning` `cs221`
