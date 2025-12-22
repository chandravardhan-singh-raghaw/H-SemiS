# H-SemiS: Hierarchical Fusion of Semi and Self-Supervised Learning for Knee Osteoarthritis Severity Grading

## Overview
This repository implements a three-stage deep learning pipeline for automated Knee Osteoarthritis (KOA) severity grading from X-ray images.

Our approach synergistically fuses self-supervised learning, semi-supervised learning, and a hybrid Quantum-Classical Convolutional Neural Network (QCNN) to leverage both labeled and unlabeled medical imaging data.

## Datasets
We use publicly available datasets for KOA grading:

### Multiclass Datasets
* [Osteoarthritis Initiative Dataset](https://data.mendeley.com/datasets/56rmx5bjcr/1)
* [Digital Knee X-ray Images](https://data.mendeley.com/datasets/t9ndx37v5h/1)

### Binary Datasets
* [Osteoarthritis Prediction Dataset](https://ieee-dataport.org/documents/osteoarthritis-prediction)
* [Knee Osteoarthritis Dataset](https://ieee-dataport.org/documents/osteoarthritis)

## Strtuctural Flow
```
├── stage_1_self_supervised_reconstruction/
│   ├── 1_data_preprocessing.ipynb
│   ├── 2_attention_unet_training.ipynb
│   ├── 3_visualization_inference.ipynb
│
├── stage_2_proxy_labeling/
│   ├── 1_feature_extraction.ipynb
│   ├── 2_similarity_labeling.ipynb
│
├── stage_3_semi_supervised_qcnn/
│   ├── 1_qcnn_model_definition.ipynb
│   ├── 2_train_hierarchical_semi_supervised.ipynb
│   ├── 3_evaluation.ipynb
```
