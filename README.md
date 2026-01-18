# Monet-Style Image Generation with GANs  
**Deep Learning – Week 5 Assignment**

![Python](https://img.shields.io/badge/python-3.11%2B-blue)
![PyTorch](https://img.shields.io/badge/pytorch-1.x-red)

---

## Overview
This repository contains the final notebook and supporting materials for the **Week 5 assignment** of the Deep Learning course.  
The project focuses on **image-to-image style transfer** in the context of the Kaggle competition *“I’m Something of a Painter Myself”*, with the objective of generating Monet-style images starting from real photographs.

The work was developed **from scratch**, strictly following the course guidelines. The emphasis is placed on **methodology, architectural reasoning, and qualitative analysis**, rather than on leaderboard performance.

---

## Scope of the Work
The notebook documents a progressive exploration of different GAN architectures:

- **DCGAN** and **WGAN-GP**, initially approached with reasonable expectations, but shown to be inadequate in their vanilla, from-scratch implementations for this task and competition setting.
- **CycleGAN**, which proved to be the most appropriate solution for unpaired image-to-image translation and produced qualitatively convincing Monet-style outputs.

The notebook includes:
- Exploratory Data Analysis (EDA) on the original Monet dataset.
- Model building and training procedures.
- Qualitative visual comparisons between real photos and generated images.
- Color distribution and saturation analysis (RGB and HSV) comparing real Monet paintings and CycleGAN outputs.
- Discussion of computational constraints and practical limitations encountered during training and submission.

---

## Results
Results are evaluated **qualitatively**, in line with the assignment objectives.  
Visual inspection and color-distribution analysis show that the CycleGAN model captures key stylistic properties of Monet paintings, particularly in terms of color tone, saturation, and global appearance.

A Kaggle submission was successfully generated, producing the required archive with **7000+ images**.  
However, the reported Kaggle score is **not representative of the actual quality of the work**, due to:
- The impossibility of using accelerated Kaggle kernels (GPU/TPU).
- The disproportionate computational cost of generating thousands of images via CPU-only execution.

The submission therefore only demonstrates that the notebook correctly generated the expected output format, which is fully consistent with the Week 5 assignment instructions, where the focus is **not** on leaderboard score but on understanding and explaining the full procedure.

---

## Reproducibility Notice
**Important**

This notebook is **not intended to be fully reproducible outside of Kaggle**.

- It was executed according to the official Kaggle notebook workflow and constraints.
- Dataset access, paths, and runtime assumptions are Kaggle-specific.
- The repository is provided for **documentation and academic evaluation purposes only**.

---

## Intended Use
This repository is intended **exclusively** for:
- Submission and evaluation within the **Deep Learning course**.
- Demonstrating understanding of GAN-based image generation and CycleGAN-style transfer.
- Academic review by instructors and peers.

No license is provided, as this repository is **not meant for reuse, redistribution, or production use**.
