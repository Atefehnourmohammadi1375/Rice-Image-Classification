# Rice Image Classification

A deep learning project for classifying rice grain images using Convolutional Neural Networks (CNNs), Transfer Learning, and Fine-Tuning with ResNet50.

## Project Overview

The objective of this project is to classify rice grain images into five different varieties:

- Arborio
- Basmati
- Ipsala
- Jasmine
- Karacadag

The dataset contains 75,000 rice grain images, with 15,000 images for each class.

Several deep learning approaches were developed and compared to investigate how architectural improvements, data augmentation, transfer learning, and fine-tuning affect classification performance.

## Models

The following models were implemented and evaluated:

1. Baseline CNN
2. Improved CNN
3. CNN with Data Augmentation
4. Improve2 CNN
5. ResNet50 Transfer Learning
6. Fine-Tuned ResNet50

## Dataset Split

The dataset was divided into:

- Training set: 60,000 images
- Validation set: 7,500 images
- Test set: 7,500 images

## Results

| Model | Test Accuracy | Misclassified Images |
|---|---:|---:|
| Baseline CNN | 98.57% | 107 |
| Improved CNN | 99.19% | 61 |
| Augmented CNN | 99.12% | 66 |
| Improve2 CNN | 99.80% | 15 |
| ResNet50 Transfer Learning | 99.64% | 27 |
| **Fine-Tuned ResNet50** | **99.89%** | **8** |

## Best Model

Fine-Tuned ResNet50 achieved the best performance in this experiment, with a test accuracy of **99.89%** and only **8 misclassified images out of 7,500 test samples**.

Fine-tuning selected layers of the pretrained ResNet50 network allowed the model to better adapt to the rice image dataset.

## Technologies

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## Conclusion

The experiments demonstrate that progressively improving the CNN architecture significantly increased classification performance.

Transfer learning with ResNet50 also achieved strong results, while fine-tuning produced the best overall performance on the test set.

The final Fine-Tuned ResNet50 model achieved **99.89% test accuracy**, making it the best-performing model evaluated in this project.
