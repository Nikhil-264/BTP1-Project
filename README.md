# 🧠 Deep Clustering for MRI Brain Tumor Classification  
### IIT Kharagpur — B.Tech Project (BTP-1)

This repository contains the implementation, report, and presentation for my **B.Tech Project (BTP-1)** titled  
**"Clustering MRI Scans Using Deep Clustering Algorithms"**  
under the guidance of **Prof. Nikita Saxena**, Department of Chemical Engineering, IIT Kharagpur.

---

## 📘 Project Overview

Brain tumors are one of the most critical neurological conditions requiring early diagnosis.  
However, labeling medical images is costly and time-consuming — hence, this project focuses on **unsupervised and semi-supervised deep clustering** of MRI brain scans to automatically discover meaningful patterns and tumor subtypes.

We combined **deep feature extraction** via a CNN-based Autoencoder with **K-Means and Gaussian Mixture Models (GMM)** for clustering in latent space, followed by **joint optimization** using both labeled and unlabeled data.

---

## ⚙️ Pipeline Architecture

1. **Data Preprocessing**
   - Skull stripping, normalization, resizing, and augmentation  
   - Improves robustness to noise and orientation

2. **Feature Extraction**
   - CNN-based Autoencoder to learn compact latent representations  

3. **Clustering Initialization**
   - K-Means on latent features for centroid initialization  
   - GMM integration for probabilistic cluster refinement  

4. **Joint Optimization**
   - Combines clustering loss (unlabeled) and cross-entropy loss (labeled)  

5. **Visualization**
   - t-SNE plots for embedding space evolution  
   - Confusion matrices for cluster quality  

---

## 📊 Results

| Metric | Value |
|--------|--------|
| Clustering Accuracy | **93.5%** |
| Silhouette Score | **0.79** |
| Improvement Over Traditional Methods | **+24%** |

### ✅ Highlights
- Identified **5 clinically relevant MRI subtypes**
- Achieved **balanced tumor detection across classes**
- Effective at distinguishing **tumor vs. non-tumor** regions  
- Reduced manual diagnostic effort and improved interpretability  

---

## 🗂️ Repository Structure

