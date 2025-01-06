# `KOL-4-GEN`: Stacked Kolmogorov-Arnold and Generative Adversarial Networks for Malware Binary Classification through Visual Analysis


Malware classification using visual analysis, which involves converting malware binaries into images to uncover class-specific patterns, is a growing research area. This paper introduces \textsc{Kol-4-Gen}, a suite of four novel deep learning models based on the `Kolmogorov-Arnold Network` (KAN) with trainable activation functions. To address potential data imbalance, a `Generative Adversarial Network` (GAN) is also employed during training. Tested on the `Malimg` (grayscale, imbalanced, 25 classes), `Malevis` (RGB, balanced, 26 classes), and `Virus-MNIST` (grayscale, imbalanced, 10 classes) datasets, the models achieved validation accuracies of approximately **99.36%**, **95.44%**, and **92.12%**, respectively, surpassing state-of-the-art methods.


![Visual Representation (grayscale) of different malware classes from the `Malimg` dataset](FIGS/malware_images.jpg)

Following are the architectural view of the 4 deep learning models proposed under `KOL-4-GEN`

![Proposed architectures for the malware classification problem through visual representation.](FIGS/models.jpg)


Following are the Confusion Matrices of the best performers (out of 4 models under `KOL-4-GEN`) for the `Malimg` (grayscale, imbalanced, 25 classes), `Malevis` (RGB, balanced, 26 classes), and `Virus-MNIST` (grayscale, imbalanced, 10 classes) datasets respectively. 


**⚠️ NOTE: The `KOL-4-GEN` models are specific to the dataset it was trained on, indicating that these models are tailored for malware classification within a particular dataset (e.g., 25 classes for `Malimg`, 26 for `Malevis`). To the best of our knowledge, no *universal malware classifier* exists, as the prevalent state-of-the-art models (e.g. DCMN by Al-Masri *et al.* [A], MFFC by Wang *et al.* [B]) remain dataset-specific.**

![Confusion Matrix (Best) on `Malimg`](CMS/CM_Malimg.jpg)

![Confusion Matrix (Best) on `Malimg`](CMS/CM_Malevis.jpg)

![Confusion Matrix (Best) on `Malimg`](CMS/CM_VirusMNIST.jpg)



# References 

[A] B. Al-Masri, N. Bakir, A. El-Zaart, and K. Samrouth, “Dual Convolutional Malware Network (DCMN): An Image-Based Malware Classification Using Dual Convolutional Neural Networks,” *Electronics*, vol. 13, no. 18, p. 3607, 2024.

[B] S. Wang, J. Wang, Y. Song, and S. Li, “Malicious code variant identification based on Multiscale Feature Fusion CNNs,” *Computational Intelligence and Neuroscience*, vol. 2021, no. 1, p. 1070586, 2021.







**FOR DATASETS (RAW + GAN BALANCED), PRETRAINED MODELS, AND OTHER SUPPLEMENTARIES VISIT https://drive.google.com/drive/folders/1VkXbmUSf1UYOKgZfFmKMxCOeYypEg5WJ**
