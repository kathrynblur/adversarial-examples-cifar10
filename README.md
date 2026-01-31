# Adversarial Examples on STL-10

A comprehensive implementation of adversarial machine learning techniques on the STL-10 dataset, demonstrating vulnerabilities of CNNs on real-world color images and exploring defense mechanisms through adversarial training.

## 📋 Overview

This repository extends adversarial machine learning research from simple datasets (MNIST) to more realistic, challenging datasets. STL-10 features 96×96 color images across 10 object classes, making it ideal for studying adversarial robustness in practical scenarios.

**Key Implementations**:
- **Baseline CNN Training** - Custom VGG-like architecture for STL-10
- **Fast Gradient Sign Method (FGSM)** - Single-step adversarial attack
- **Adversarial Training** - Defense mechanism through robust optimization
- **Comprehensive Evaluation** - Multiple epsilon values (1/255 to 8/255)
- **Visualization** - Side-by-side comparison of clean and adversarial examples

## 🎯 Key Features

- ✅ Production-ready PyTorch implementation
- ✅ Detailed Jupyter notebook
- ✅ STL-10 dataset handling (96×96 RGB images)
- ✅ FGSM attack with configurable perturbation budgets
- ✅ Adversarial training for improved robustness

## 📁 Repository Structure

```
.
├── adversarial_examples_stl10_enhanced.ipynb  # Main notebook with full implementation
├── README.md                                   # This file
```


## 📊 Dataset: STL-10

**STL-10** (Stanford Tiny ImageNet-10) is a recognition dataset for developing unsupervised learning algorithms:

| Property | Value |
|----------|-------|
| Image size | 96×96 pixels (RGB) |
| Classes | 10 objects |
| Train set | 5,000 labeled images (500/class) |
| Test set | 8,000 labeled images (800/class) |
| Unlabeled | 100,000 images (not used here) |

**Classes**: airplane, bird, car, cat, deer, dog, horse, monkey, ship, truck

**Why STL-10 for Adversarial Research?**
- More realistic than MNIST (real photographs vs handwritten digits)
- Higher resolution challenges (96×96 vs 28×28)
- Color complexity (3 channels vs 1)
- Limited training data (tests generalization under constraint)


## 📚 References

### Foundational Papers

1. **Goodfellow et al. (2015)** - "Explaining and Harnessing Adversarial Examples"
   - Introduced FGSM attack
   - Proposed adversarial training
   - Linear explanation of adversarial phenomena

2. **Madry et al. (2018)** - "Towards Deep Learning Models Resistant to Adversarial Attacks"
   - PGD attack (projected gradient descent)
   - Min-max robust optimization framework
   - Current standard for adversarial training


### Dataset

4. **Coates et al. (2011)** - "An Analysis of Single-Layer Networks in Unsupervised Feature Learning"
   - Introduced STL-10 dataset
   - Designed for unsupervised learning


## 🙏 Acknowledgments

- Implementation based on foundational work by Goodfellow, Madry, and colleagues
- STL-10 dataset from Adam Coates et al.
- PyTorch framework for deep learning
- Community-standard epsilon values for RGB adversarial examples

---

**Note**: STL-10's limited training data (500 images/class) makes it particularly challenging. Production systems would benefit from larger datasets, extensive data augmentation, and more sophisticated architectures.
