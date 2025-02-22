# KMNIST_ResNet_FineTuning

This repository implements a deep learning solution to classify handwritten Japanese characters from the KMNIST dataset using a pre-trained ResNet50 model. The project demonstrates how to use transfer learning and fine-tuning techniques to improve model accuracy.

## Features

- **Dataset Preprocessing**: 
  - Converts grayscale images to RGB format.
  - Resizes images to 64x64 pixels.
  - Normalizes pixel values between 0 and 1.
  
- **Model Architecture**:
  - Uses ResNet50 pre-trained on ImageNet as the base model.
  - Adds custom layers for classification.
  - Fine-tunes specific layers after initial training.

- **Training**:
  - The model is first trained using the base layers of ResNet50 frozen, followed by fine-tuning to adjust some of the higher layers.

- **Evaluation**:
  - Validates the model’s performance using accuracy metrics.
  - Generates and visualizes a confusion matrix to show classification results.

## Installation

To set up the environment and run the project, ensure you have Python 3.6+ installed, then use the following commands:

```bash
pip install tensorflow numpy matplotlib seaborn scikit-learn
