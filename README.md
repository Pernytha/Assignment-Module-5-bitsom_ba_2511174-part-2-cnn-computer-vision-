##  Computer Vision Problem Formulation and CNN Prototype

## Project Title

**Computer Vision Problem Formulation and CNN Prototype**

## Approach

The project uses a Convolutional Neural Network (CNN) to classify images by learning visual patterns through preprocessing, training and evaluation.


## Problem Statement

The objective of this project is to build a **Convolutional Neural Network (CNN)** that can classify images into different categories.

The model learns patterns from images and predicts the correct class label for unseen images.


##  Dataset Description

The dataset consists of images organized into class-specific folders. Each folder represents one category.

- Each image belongs to only one class
- The task is a multi-class image classification problem

### Dataset Link:
https://drive.google.com/drive/folders/1akV6po4Nrgkc3yQrJkzA6cJIV-wBvUYs?usp=sharing

## Steps Followed


### 1.Data Preprocessing

- Resized images to **128 × 128 pixels**
- Normalized pixel values from **[0, 255] → [0, 1]**
- Split dataset into:
  - Training set (80%)
  - Testing/Validation set (20%)
- Applied data augmentation:
  - Rotation
  - Zoom
  - Horizontal flipping


### 2. Model Building

A CNN model was built using:

- Convolution layers (feature extraction)
- ReLU activation function
- MaxPooling layers (dimensionality reduction)
- Flatten layer
- Dense fully connected layers
- Softmax output layer for classification


### 3.Training

- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Metric: Accuracy
- Model trained for multiple epochs

Training and validation accuracy were monitored during training.


### CNN Concept Explanation

# What is Convolution?

Convolution is a process where a small filter (kernel) moves across an image to extract important features such as edges, textures, and patterns.  
It helps the model understand visual structures in an image.


# Why is Pooling used?

Pooling is used to reduce the spatial size of feature maps while keeping important information.

It helps in:
- Reducing computation cost
- Preventing overfitting
- Making the model more efficient


# Why is ReLU commonly used in CNNs?

ReLU (Rectified Linear Unit) is used as an activation function because:

- It introduces non-linearity
- It helps the model learn complex patterns
- It avoids the vanishing gradient problem
- It speeds up training

ReLU converts negative values to zero and keeps positive values unchanged.

# Why are CNNs better than regular feed-forward networks for image data?

CNNs are better because:

- They preserve spatial relationships in images
- They use shared weights, reducing the number of parameters
- They automatically learn features (edges → shapes → objects)
- They are more efficient for high-dimensional image data

In contrast, feed-forward networks treat all pixels independently and lose spatial structure.



### 4. Results

The model was evaluated using:

- Training accuracy
- Validation accuracy
- Test accuracy
- Confusion matrix
- Accuracy/Loss graphs

### Output Files:
- `results/accuracy_loss_curves.png`
- `results/confusion_matrix.png`
- `sample_predictions/prediction_outputs.png`

### Performance:
- Training Accuracy: *(add value)*
- Validation Accuracy: *(add value)*
- Test Accuracy: *(add value)*


## Observations & Insights

- CNN successfully learned patterns from image data
- More training data improves model performance
- Some classes may be confused if visually similar
- Data augmentation improves generalization
- Slight overfitting may occur if model is too complex



## Conclusion

This project demonstrates how CNNs can effectively solve image classification problems by learning hierarchical features from images.

CNNs are widely used in real-world applications such as:
- Healthcare (medical imaging)
- Retail (product classification)
- Agriculture (crop disease detection)
- Security systems

