# Concrete Crack Detection Using Deep Learning

A deep learning-based image classification project that detects cracks in concrete surfaces using a custom Convolutional Neural Network (CNN) built with PyTorch.

## Project Overview

This project explores automated concrete crack detection using computer vision and deep learning.

A custom CNN is trained to classify concrete surface images into two categories:

- **Positive (1):** Cracked concrete
- **Negative (0):** Crack-free concrete

The project also investigates the impact of class imbalance and compares standard training with weighted loss.

## Objectives

- Develop a CNN-based concrete crack classification model.
- Preprocess and augment concrete surface images.
- Study the effect of class imbalance on model performance.
- Compare standard loss with weighted loss.
- Evaluate models using classification metrics and Precision-Recall curves.

## Dataset

**Dataset:** Concrete Crack Images for Classification – Kaggle

- Total available images: 40,000
- Negative images: 20,000
- Positive images: 20,000
- Selected images for the experiment: 8,000

The selected dataset was divided into training, validation and testing sets.

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

## Methodology

1. Load and explore the concrete crack image dataset.
2. Resize images to 128 × 128 pixels.
3. Apply image preprocessing and data augmentation.
4. Build and train a custom CNN.
5. Create an imbalanced training scenario.
6. Apply class-weighted loss to address class imbalance.
7. Compare baseline and weighted-loss models.
8. Evaluate performance using classification metrics and Precision-Recall curves.

## Model Performance

| Metric | Baseline CNN | Weighted Loss CNN |
|---|---:|---:|
| Accuracy | 99.58% | 99.25% |
| Precision | 99.83% | 98.84% |
| Recall | 99.33% | 99.67% |
| F1-score | 99.58% | 99.25% |
| Specificity | 99.83% | 98.83% |
| Average Precision | 99.99% | 99.95% |

### Key Observation

Weighted loss improved crack detection recall from 99.33% to 99.67%, while slightly reducing overall accuracy.

This experiment demonstrates how class weighting can influence model performance when training data is imbalanced.

## Limitations and Future Scope

- Evaluate on larger and more diverse concrete image datasets.
- Test performance under different lighting and surface conditions.
- Experiment with advanced CNN architectures.
- Explore object detection and segmentation for crack localization.
- Validate performance on independent real-world industrial images.

## How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Download the dataset from Kaggle.
4. Update the dataset directory in the notebook.
5. Open the notebook in Google Colab or Jupyter Notebook.
6. Run the cells sequentially.

## Disclaimer

This project was developed for academic and educational purposes. Its reported performance is based on the selected experimental dataset and should not be interpreted as a guarantee of real-world industrial performance.
