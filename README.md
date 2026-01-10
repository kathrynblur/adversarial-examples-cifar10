# Adversarial Examples on CIFAR-10

This repo explores adversarial examples on CIFAR-10 using the FGSM attack and adversarial training.
It is adapted from my earlier MNIST adversarial-examples notebook, but updated for a 3-channel, higher-variance dataset.
The model trained isn't sophisticated at all and has a comparably low accuracy due to a particular focus on adversarial examples. More complex models would perform better on average with adversarial examples, while this model reveals how adversarial examples can affect accuracy.

## What’s inside
- Baseline CNN training on CIFAR-10
- FGSM attack + evaluation
- Adversarial training + robustness comparison
- Visualizations of perturbations and misclassifications

## Results (quick summary)
- Clean accuracy: TODO
- FGSM accuracy (ε=1/255): TODO

## Repo structure
- `notebook/` : runnable notebooks in a narrative order


