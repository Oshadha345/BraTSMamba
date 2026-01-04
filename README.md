# 🧠 BraTSMamba: SegMamba 3D Segmentation

> **System Status**: `ONLINE`  
> **Architecture**: `BraTSMamba`  
> **Target**: `Brain Tumor Segmentation (BraTS)`

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![MONAI](https://img.shields.io/badge/MONAI-1.3%2B-purple?style=for-the-badge&logo=monai&logoColor=white)](https://monai.io/)
[![Mamba](https://img.shields.io/badge/Mamba-SSM-yellow?style=for-the-badge&logo=snake&logoColor=black)](https://github.com/state-spaces/mamba)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![Code Style](https://img.shields.io/badge/Code%20Style-Black-000000?style=for-the-badge&logo=code-review&logoColor=white)](https://github.com/psf/black)

</div>

---

## 🏗️ Model Architecture

The core architecture leverages the efficiency of Conv3D combined with the global context modeling capabilities of Mamba state-space blocks.

![BraTSMamba Architecture](Model%20Architecture/BraTSMamba_final.jpg)

---

## 📊 Results & Evaluation

Our BraTSMamba model achieves state-of-the-art performance on the BraTS 2021 dataset.

### 📈 Quantitative Metrics

| Region | Dice Score (DSC) | HD95 (mm) |
| :--- | :---: | :---: |
| **Whole Tumor (WT)** | **0.909** | **6.70** |
| **Tumor Core (TC)** | **0.884** | **5.44** |
| **Enhancing Tumor (ET)** | **0.857** | **3.80** |
| **Mean** | **0.883** | **-** |

### 📉 Training Performance

![Training Curves](Results/BraTSMamba%20Evaluation/training_curves.png)

### 🖼️ Qualitative Results

Visual comparison of Ground Truth vs. Model Prediction:

<div align="center">
  <img src="Results/BraTSMamba%20Evaluation/error_analysis_sample_0.png" width="45%" alt="Sample 0" />
  <img src="Results/BraTSMamba%20Evaluation/error_analysis_sample_2.png" width="45%" alt="Sample 2" />
</div>

### 📂 Dataset Analysis

Understanding the data distribution and modalities:

<div align="center">
  <img src="Results/raw_dataset_results/BraTS_all_modalities.png" width="80%" alt="Modalities" />
</div>

<div align="center">
  <img src="Results/raw_dataset_results/class_distribution_pie.png" width="45%" alt="Class Distribution" />
  <img src="Results/raw_dataset_results/tumor_volume_distribution.png" width="45%" alt="Volume Distribution" />
</div>

---

## 📓 Detailed Reports

For a deep dive into the methodology, experiments, and detailed error analysis, please refer to:

*   📘 **[BioMamba Project Report](BioMamba_Report.pdf)**
*   📓 **[Interactive Notebook](BioMamba_Notebook.ipynb)**

---

## 🏆 Competition Guide

For detailed guidelines and the framework of the competition, please refer to the delegate booklet:

*   📄 **[Delegate Booklet: Guidelines and Competition Framework](Competition%20Guide/DELEGATE%20BOOKLET%20_%20Guidelines%20and%20competition%20framework.pdf)**

---

## 📚 Research Papers

The following research papers provide the foundational knowledge and state-of-the-art methods used in this project:

### Core Mamba Papers
*   **[Mamba: Linear-Time Sequence Modeling with Selective State Spaces](Research%20Papers/2312.00752v2.pdf)** (2312.00752)
*   **[SegMamba: Long-range Sequential Modeling Mamba For 3D Medical Image Segmentation](Research%20Papers/2401.13560v4.pdf)** (2401.13560)
*   **[U-Mamba: Enhancing Long-range Dependency for Biomedical Image Segmentation](Research%20Papers/2401.04722v1.pdf)** (2401.04722)
*   **[MedSegMamba: 3D CNN-Mamba Hybrid Architecture for Brain Segmentation](Research%20Papers/2409.08307v3.pdf)** (2409.08307)

### Foundational Segmentation Papers
*   **[3D U-Net: Learning Dense Volumetric Segmentation from Sparse Annotation](Research%20Papers/1606.06650v1.pdf)** (1606.06650)
*   **[nnU-Net for Brain Tumor Segmentation](Research%20Papers/2011.00848v1.pdf)** (2011.00848)
*   **[Swin UNETR: Swin Transformers for Semantic Segmentation of Brain Tumors in MRI Images](Research%20Papers/2201.01266v1.pdf)** (2201.01266)

---

<div align="center">
<sub>Built with 💻 and ☕ by the BioMamba Team</sub>
</div>
