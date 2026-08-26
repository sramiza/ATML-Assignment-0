# ATML Assignment 0: Deep Learning Foundations

**Author:** Syed Ramiz Abbas  
**Course:** Advanced Topics in Machine Learning (ATML)  

## Overview
This repository contains the code, experiments, and final report for Assignment 0. The project breaks down the inner mechanics of four distinct deep learning architectures, focusing on feature transferability, attention routing, multimodal contrastive alignment, and generative modeling.

## Project Structure
The assignment is divided into four core experiments:

*   **Task 1: Convolutional Transfer Learning (ResNet-152):** 
    Evaluates the transferability of ImageNet features to CIFAR-10. Includes an ablation study on residual skip connections to observe gradient flow collapse, and t-SNE visualizations of feature hierarchies across network depth.
*   **Task 2: Vision Transformers (ViT):** 
    Explores global self-attention routing. Includes structural occlusion experiments (random vs. center-block masking) and compares the linear separability of the `[CLS]` token bottleneck against mean-pooled patch representations.
*   **Task 3: Multimodal Contrastive Learning (CLIP):** 
    Analyzes zero-shot classification on the STL-10 dataset using prompt engineering. Includes patch-level cosine similarity heatmaps and applies Orthogonal Procrustes alignment to bridge the Euclidean modality gap between image and text embeddings.
*   **Task 4: Variational Autoencoders (VAE):** 
    Implements a baseline VAE to model the generative distribution of the MNIST dataset. Maps embeddings to a strictly constrained 2D latent manifold to evaluate the trade-offs between reconstruction sharpness and continuous generative sampling.

## Installation & Setup
To run the experiments locally, clone this repository and install the required dependencies:

```bash
git clone [https://github.com/sramiza/ATML-Assignment-0.git](https://github.com/sramiza/ATML-Assignment-0.git)
cd ATML-Assignment-0
pip install -r requirements.txt
