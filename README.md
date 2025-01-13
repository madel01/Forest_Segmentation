# Forest_Segmentation
### Forest scenes Segmentation in Aerial images using Residual Unet

This repository contains the implementation of **Forest Segmentation** using the **Res-UNet** architecture. The project focuses on accurately segmenting forest areas from satellite images using deep learning techniques.

## Dataset

The dataset used in this project is sourced from Kaggle:  
[Augmented Forest Segmentation Dataset](https://www.kaggle.com/datasets/quadeer15sh/augmented-forest-segmentation)

The dataset includes preprocessed satellite images and corresponding mask labels to train, validate, and test the model.

---

## Model Architecture

The **Res-UNet** (Residual UNet) architecture combines the strengths of the UNet model for segmentation tasks and residual connections to address vanishing gradient issues. This architecture ensures efficient feature extraction and improved segmentation performance.  

### Key Features:
- **Encoder-Decoder Architecture**: Extracts hierarchical features from input images and reconstructs them for pixel-level segmentation.
- **Residual Connections**: Enhances gradient flow and network training by bypassing signals.
- **Skip Connections**: Transfers high-resolution spatial information between encoder and decoder paths.

---

## Project Workflow

1. **Data Preparation**:
   - Preprocessing images (normalization, resizing).
   - Data Augmentation using "albumentation" package.

2. **Model Implementation**:
   - Building the Res-UNet model using a deep learning framework (e.g., TensorFlow/Keras or PyTorch).
   - Configuring hyperparameters such as learning rate, batch size, and optimizer.

3. **Training**:
   - Training the Res-UNet model on the dataset.
   - Using data augmentation techniques to improve generalization.

4. **Evaluation**:
   - Evaluating the model on validation and test sets.
   - Metrics used: Dice Coefficient, Intersection over Union (IoU), Precision, Recall.

5. **Inference**:
   - Generating segmentation masks on unseen satellite images.

---

## Results

The Res-UNet model achieves high accuracy in segmenting forest areas, demonstrating its effectiveness for satellite imagery tasks. Quantitative results include:

- **IoU**: ~0.67

