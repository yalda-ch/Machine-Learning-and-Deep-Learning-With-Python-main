# Project 4 --- Handwritten Character Recognition with EMNIST

**Notebook:** `Yalda_Chamani_Project4.ipynb`\
**Folder:** `project 4`

------------------------------------------------------------------------

## 📌 Project Description

This project implements a **Convolutional Neural Network (CNN)** for
handwritten character recognition using the **EMNIST (Extended MNIST)**
dataset. It also integrates **Weights & Biases (wandb)** for experiment
tracking and performs **hyperparameter tuning** to improve performance.

------------------------------------------------------------------------

## 📊 Dataset

-   **Dataset:** EMNIST (Balanced split)\
-   **Classes:** 47 balanced handwritten characters\
-   **Splits:**
    -   80% Training set\
    -   20% Validation set\
    -   Separate Test set

Each image:\
- **28×28 grayscale handwritten character**\
- **Label:** corresponding class from EMNIST

------------------------------------------------------------------------

## 🛠️ Tools & Libraries

-   Python 3.x\
-   PyTorch (torch, torch.nn, torch.optim, DataLoader)\
-   Torchvision (EMNIST, transforms)\
-   Matplotlib\
-   NumPy\
-   tqdm (progress tracking)\
-   scikit-learn (confusion_matrix, ConfusionMatrixDisplay)\
-   **Weights & Biases (wandb)** for experiment tracking

------------------------------------------------------------------------

## 🚀 Workflow

1.  **Dataset Preparation** --- Download EMNIST, apply transformations
    (tensor conversion, normalization).\
2.  **Data Splitting** --- Divide into training, validation, and test
    sets.\
3.  **Visualization** --- Display sample images from dataset.\
4.  **CNN Model Design** ---
    -   Convolutional layers with ReLU + MaxPooling\
    -   Fully connected layers with Dropout\
    -   Customizable parameters (filters, kernel size, dropout).\
5.  **Training & Validation** --- Implement `train_step` and `test_step`
    loops with loss and accuracy tracking.\
6.  **Experiment Tracking** --- Log metrics, confusion matrices, and
    hyperparameters with **wandb**.\
7.  **Evaluation** --- Assess accuracy and visualize confusion matrix on
    test set.

------------------------------------------------------------------------

## 📈 Results

-   The **baseline CNN** achieved strong classification accuracy on the
    EMNIST balanced dataset, demonstrating the effectiveness of
    convolutional layers for handwritten character recognition.\
-   **Experiment tracking with wandb** provided detailed insights into
    model behavior, including real-time loss/accuracy curves, learning
    rate schedules, and comparison across multiple runs.\
-   **Hyperparameter tuning** (e.g., varying number of filters, kernel
    size, and dropout rate) led to measurable improvements in validation
    accuracy and reduced overfitting.\
-   The **best model configuration** achieved the highest accuracy on
    the test set, confirming the benefit of systematic optimization.\
-   **Confusion matrices** revealed common misclassifications (e.g.,
    visually similar characters), offering useful insights for further
    model refinement.

------------------------------------------------------------------------

## 🎯 Learning Outcome

-   Build a **CNN model** for image classification in PyTorch.\
-   Understand **data preprocessing and normalization** for image
    datasets.\
-   Gain experience with **wandb for experiment tracking**.\
-   Learn how **hyperparameter tuning** impacts deep learning
    performance.\
-   Visualize results with **confusion matrices and sample outputs**.
