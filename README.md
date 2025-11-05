# Face_Recognition_Occluded_Images_Enchanced_GAN
This project presents a comprehensive comparative study on improving facial recognition accuracy when faces are partially occluded by objects such as masks, hands, or glasses. The study evaluates four approaches: Direct on Clean Faces and Occluded Faces then using Basic GAN and Enhanced GAN 

This project focuses on improving face recognition accuracy when facial regions are partially covered (by masks, hands, or glasses).
It compares different recognition methods and introduces an Enhanced Perceptual Conditional GAN (P-cGAN) for reconstructing occluded faces with high identity preservation.

Overview

The system evaluates four approaches:
Direct Recognition (clean faces)
Recognition on Occluded Faces
Reconstruction using Basic Conditional GAN (cGAN)
Reconstruction using Enhanced Perceptual cGAN (P-cGAN)

The proposed Enhanced GAN integrates perceptual loss (VGG19), a feature-matching discriminator, and Gaussian noise regularization, producing more realistic and identity-consistent face reconstructions.

⚙️ Tech Stack

Language: Python

Frameworks: TensorFlow, Keras

Models: U-Net Generator, PatchGAN Discriminator, MobileNetV2 (recognition)

Dataset: ~1,400 paired clean and occluded face images (from Kaggle Face Mask Detection)
| Dataset                         | Accuracy (%) |
| ------------------------------- | ------------ |
| Clean Faces                     | 96.1         |
| Occluded Faces                  | 57.3         |
| Basic GAN Reconstruction        | 78.4         |
| **Enhanced GAN Reconstruction** | **94.2**     |
