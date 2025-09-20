#  Image Classification with Convolutional Neural Networks (CNN)

This project demonstrates how to build, train, and evaluate a
**Convolutional Neural Network (CNN)** to classify images of **cats
vs. dogs** using TensorFlow/Keras. The dataset is a subset of the Kaggle
**Dogs vs. Cats** dataset, containing 2,000 images.

------------------------------------------------------------------------

##  Project Overview

The project covers: 1. Exploring and preparing image data. 2. Building
and training a CNN for binary image classification. 3. Evaluating the
performance on training and validation datasets.

------------------------------------------------------------------------

##  Dataset

-   **Source**: [Dogs vs. Cats dataset
    (Kaggle)](https://www.kaggle.com/c/dogs-vs-cats/data)

-   **Subset used**: 2,000 images (to reduce training time).

-   **Structure**:

        cats_and_dogs_filtered/
        ├── train/
        │   ├── cats/
        │   └── dogs/
        └── validation/
            ├── cats/
            └── dogs/

-   **Note**: Images are automatically labeled by their folder name
    using **ImageDataGenerator**.

------------------------------------------------------------------------

## Tech Stack

-   **Python**
-   **TensorFlow / Keras** (CNN model building and training)
-   **NumPy, Matplotlib** (data manipulation and visualization)

------------------------------------------------------------------------

##  Implementation Steps

1.  **Load and explore data**
    -   Download dataset and unzip to `/cats_and_dogs_filtered/`.
    -   Inspect training and validation directories.
2.  **Preprocessing**
    -   Use **ImageDataGenerator** to:
        -   Rescale images (normalize pixel values).
        -   Automatically assign labels based on folder names.
3.  **Build CNN model**
    -   A typical CNN architecture may include:
        -   Convolutional layers
        -   MaxPooling layers
        -   Flatten layer
        -   Dense layers
        -   Output layer with sigmoid activation (binary classification)
4.  **Compile model**
    -   Optimizer: `adam`
    -   Loss: `binary_crossentropy`
    -   Metrics: `accuracy`
5.  **Train the model**
    -   Fit the model with training data.
    -   Validate on validation set.
6.  **Evaluate performance**
    -   Track accuracy and loss for both training and validation sets.
    -   Visualize results with accuracy/loss plots.

------------------------------------------------------------------------

##  Evaluation

-   Model performance is measured using:
    -   **Training accuracy**
    -   **Validation accuracy**
-   Helps assess how well the CNN generalizes to unseen data.
