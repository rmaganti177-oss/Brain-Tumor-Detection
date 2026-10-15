# Brain Tumor Detection Using 2D CNN

## Overview

Brain Tumor Detection Using 2D CNN is an AI-based medical image classification project that uses a Convolutional Neural Network (CNN) to classify brain MRI images into four categories:

1. **Glioma**
2. **Meningioma**
3. **No Tumor**
4. **Pituitary**

The project explores deep learning techniques for brain MRI image classification. It predicts the category of an input MRI image and, if supported by the implementation, displays the predicted class and confidence score.

## Features

- **Four-Class Classification:** Classifies MRI images into Glioma, Meningioma, No Tumor, and Pituitary categories.
- **CNN-Based Model:** Uses a 2D Convolutional Neural Network for image classification.
- **Image Preprocessing:** Resizes MRI images to 255 × 255 pixels.
- **Data Augmentation:** Uses rotation, flipping, and zooming to augment training images.
- **Prediction Confidence:** Displays prediction confidence if implemented in the application.
- **Results Visualization:** Provides prediction outputs and image visualizations supported by the project.

## Model Architecture

The CNN model architecture includes the following components:

- **Convolutional Layers:** Extract important features from MRI images.
- **Max Pooling Layers:** Reduce spatial dimensions and computational complexity.
- **Dropout Layers:** Help reduce overfitting during training.
- **Fully Connected Layers:** Learn relationships between extracted features for classification.
- **Softmax Activation:** Produces class probability scores for multi-class classification.

## Performance Metrics

The following performance figures were reported for the model:

| Metric | Reported Result |
|---|---:|
| Training Accuracy | 96.73% |
| Test Accuracy | 96.72% |
| Test Loss | 0.0836 |
| Validation Accuracy | 97.71% |

These values should be interpreted according to the dataset split and evaluation methodology used during training.

## Dataset

The project uses the Brain Tumor MRI Dataset available on Kaggle.

**Dataset link:** [Brain Tumor MRI Dataset — Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)

The dataset contains labeled brain MRI images belonging to four categories: Glioma, Meningioma, No Tumor, and Pituitary.

Download and extract the dataset into `Implementation/dataset/` so it contains the `Training/` and `Testing/` folders expected by the notebook.

Please review the dataset's license and terms before redistributing its images.

## Dataset Preprocessing

The reported preprocessing and augmentation steps include:

1. **Image Resizing:** Resizing MRI images to 255 × 255 pixels.
2. **Rotation:** Applying rotations to create variations in training images.
3. **Flipping:** Generating flipped images for data augmentation.
4. **Zooming:** Applying zoom transformations to introduce image variations.

The preprocessing configuration used during inference should match the configuration expected by the trained model.

## Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn
- Convolutional Neural Networks (CNN)

## Installation

### Prerequisites

- Python installed on your system
- pip package manager
- Git

### Step 1: Clone the Repository

```bash
git clone https://github.com/rmaganti177-oss/Brain-Tumor-Detection.git
cd Brain-Tumor-Detection
```

### Step 2: Install Dependencies

```bash
python -m pip install --upgrade pip
pip install tensorflow opencv-python matplotlib numpy scikit-learn keras
```

**Note:** Package versions may need to be adjusted to match the Python version and TensorFlow version used to train the model.

### Step 3: Run the Project

Open the project folder in VS Code or your preferred Python IDE.

Run the notebook or Python script provided in the repository according to the project's file structure. If the repository includes a Jupyter notebook, you can install and launch Jupyter with:

```bash
pip install notebook
jupyter notebook
```

Then open the relevant notebook and execute its cells in order.

## Results Visualization

The project describes visualization of predicted tumor regions using bounding circles on MRI images, along with the predicted class and confidence score.

**Important:** A standard image-classification CNN does not automatically localize a tumor. Bounding circles represent meaningful tumor localization only if an additional localization or image-processing method is implemented and validated.

## References

1. [Brain Tumor MRI Dataset — Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)
2. [BMC Medical Informatics and Decision Making — Research Article](https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/s12911-023-02114-6)
3. [IEEE Xplore — Research Paper](https://ieeexplore.ieee.org/document/8934561)
4. [PubMed Central — Research Article](https://pmc.ncbi.nlm.nih.gov/articles/PMC10527911/)

## Medical Disclaimer

This project is intended for educational and research purposes only. It is not a clinically validated diagnostic tool and must not be used as a substitute for professional medical advice, diagnosis, or treatment. MRI results should be interpreted by qualified healthcare professionals.

## Repository

GitHub: [rmaganti177-oss/Brain-Tumor-Detection](https://github.com/rmaganti177-oss/Brain-Tumor-Detection)

Related project: [AI-Based Disease Diagnostic](https://github.com/rmaganti177-oss/AI-Based-Disease-Diagnostic)