# Facial Image Colorization Using Pix2Pix

This project explores **automatic colorization of grayscale facial images** using the **Pix2Pix architecture**, a conditional Generative Adversarial Network (cGAN) designed for paired image-to-image translation tasks.

## Overview
The system employs a **U-Net-based generator** with skip connections and a **PatchGAN discriminator** to reconstruct realistic chrominance information from luminance inputs.  
Training stability and convergence were enhanced through techniques such as **label smoothing**, **label flipping**, and **progressive learning rate decay**.

The model was trained and evaluated on a reduced version of the **CelebA** dataset (25,000 aligned face images), converted to the **CIELAB color space** for explicit luminance–chrominance separation.

## Key Features
- **Pix2Pix (cGAN)** architecture optimized for face colorization;  
- **U-Net generator + PatchGAN discriminator** design;  
- Advanced training stabilization (label smoothing, label flipping, learning rate decay);  
- Quantitative and perceptual evaluation using **PSNR, SSIM, ΔE, and Chroma Accuracy**;  
- High-quality, perceptually coherent colorization results.  

## Results
The model achieved the following average results on the test set:

| Metric | Value |
|:-------:|:------:|
| **PSNR** | 26.18 dB |
| **SSIM** | 0.9455 |
| **ΔE** | 10.72 |
| **Chroma Accuracy** | 0.60 |

These results confirm that the optimized Pix2Pix implementation produces **realistic, structurally faithful, and chromatically consistent** facial colorizations.

## Applications
- Restoration of historical or grayscale photographs;  
- Creative and media content generation;  
- Automated facial image enhancement.  

## Authors
- Anita Ascheri    
- Ilaria Sarcuni  
  
