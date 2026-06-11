# CLASSIFICATION-AND-EXPLAINABLE-ANALYSIS-OF-COMPRESSED-IMAGES-USING-ADVANCED-NEURAL-NETWORKS-AND-LLMS

## B.Tech Major Project

This repository contains the implementation, project report, and research paper for our B.Tech Major Project focused on investigating the effect of image compression on deep learning-based diabetic retinopathy classification.

## Project Overview

Diabetic Retinopathy (DR) is one of the leading causes of vision loss worldwide. Automated diagnosis using deep learning has shown promising results; however, medical image storage and transmission remain challenging due to large image sizes.

This project explores how image compression affects classification performance by combining an SVD-based image compression technique with a Depthwise Separable Convolutional Neural Network (DS-CNN).

The primary objective is to evaluate whether compressed retinal images can maintain sufficient diagnostic information for accurate diabetic retinopathy classification.

---

## Research Objectives

* Investigate the impact of image compression on diabetic retinopathy classification performance.
* Develop an SVD-based sparse sampling compression framework.
* Evaluate the robustness of DS-CNN models on compressed retinal fundus images.
* Analyze the trade-off between compression ratio and classification accuracy.

---

## My Contribution

As part of this major project, my primary responsibility was:

* Researching and identifying a suitable image compression technique for the problem.
* Studying various compression approaches and selecting Singular Value Decomposition (SVD) as the most appropriate method.
* Implementing the SVD-based sparse sampling compression algorithm.
* Integrating the compression pipeline with the classification workflow.
* Evaluating how different compression levels influence model performance.
* Contributing to the preparation of the research paper and project documentation.

---

## Dataset

### APTOS 2019 Blindness Detection Dataset

The experiments were conducted using the APTOS 2019 Blindness Detection dataset from Kaggle.

Dataset Characteristics:

* Source: APTOS 2019 Blindness Detection Competition
* Image Type: Color retinal fundus images
* Total Images: 3,662
* Training Images: 2,931
* Validation Images: 731
* Classes: 5

Classification Categories:

| Label | Diabetic Retinopathy Stage |
| ----- | -------------------------- |
| 0     | No DR                      |
| 1     | Mild                       |
| 2     | Moderate                   |
| 3     | Severe                     |
| 4     | Proliferative DR           |

---

## Methodology

### SVD-Based Image Compression

The proposed compression framework uses Singular Value Decomposition (SVD) with sparse sampling of singular vectors.

Compression Process:

1. Perform SVD decomposition of the image.
2. Extract important key points from singular vectors.
3. Store sparse representations of U and V matrices.
4. Preserve singular values.
5. Reconstruct images through interpolation during decompression.

Advantages:

* Higher compression ratios.
* Better preservation of structural information.
* Reduced storage requirements.
* Minimal degradation in classification performance.

---

## Training Configuration

* Framework: TensorFlow/Keras
* Optimizer: Adam
* Learning Rate: 0.001
* Loss Function: Categorical Cross-Entropy
* Epochs: 26
* Batch Size: 32
* Validation Split: 20%
* Hardware: Google Colab (NVIDIA T4 GPU)

Class imbalance was handled using balanced class weights.

---

## Repository Structure

```
├── model.py             # SVD-based compression implementation  # DS-CNN training pipeline  # Performance evaluation
├── report/
│   └── BTech_Major_Project_Report.pdf
├── research_paper/
│   └── Research_Paper.pdf
├── requirements.txt
└── README.md
```

---

## Research Paper

This repository also includes the research paper developed as part of this project, presenting the methodology, experimental findings, and analysis of compressed-domain diabetic retinopathy classification.

---

## Technologies Used

* Python
* TensorFlow/Keras
* NumPy
* SciPy
* Scikit-learn
* Matplotlib
* Seaborn
* Google Colab
* NVIDIA T4 GPU

---

## Disclaimer

The APTOS 2019 dataset is publicly available through Kaggle and should be used in accordance with its licensing terms. This repository is intended solely for academic and research purposes.

---

## Citation

If you use this work in your research, please cite the accompanying research paper provided in this repository.

---

## Acknowledgements

* APTOS 2019 Blindness Detection Competition
* Kaggle
* Faculty mentors and project supervisors who guided this work throughout the research process.

---

**B.Tech Major Project – Department of Information Technology**

**Author:** Deepanshu Singh , Dev Sharma and Devyash Jain
