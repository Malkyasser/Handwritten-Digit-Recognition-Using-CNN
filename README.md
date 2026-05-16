# Handwritten-Digit-Recognition-Using-CNN
# Handwritten Digit Recognition using CNN

## Project Description

This project implements a Convolutional Neural Network (CNN) using PyTorch for handwritten digit recognition on the MNIST dataset.

The project compares two experiments using different optimizers:
- Adam Optimizer
- SGD Optimizer

The performance of both models is evaluated using:
- Accuracy
- Loss

Training and validation curves are also visualized.

---

# Dataset

Dataset used:
MNIST Handwritten Digits Dataset

The dataset contains:
- 60,000 training images
- 10,000 testing images
- 10 classes (digits from 0 to 9)

Dataset Link:
https://yann.lecun.com/exdb/mnist/

---

# Project Steps

## 1. Import Libraries

Required libraries such as:
- torch
- torchvision
- matplotlib

were imported for deep learning, dataset loading, and visualization.

---

## 2. Data Preprocessing

The following preprocessing techniques were applied:
- Convert images to tensors using `ToTensor()`
- Normalize image values using `Normalize()`

This helps improve model training performance.

---

## 3. Load Dataset

The MNIST dataset was loaded using `torchvision.datasets.MNIST`.

The dataset was automatically divided into:
- Training dataset
- Testing dataset

DataLoader was used to create batches and shuffle training data.

---

## 4. Build CNN Model

A simple CNN architecture was implemented using:
- Convolutional layers
- ReLU activation functions
- MaxPooling layers
- Fully Connected layers
- Dropout layer

The CNN extracts important image features and classifies handwritten digits.

---

# CNN Architecture

```text
Input Image (28x28)

→ Conv2D
→ ReLU
→ MaxPooling

→ Conv2D
→ ReLU
→ MaxPooling

→ Flatten

→ Fully Connected Layer
→ ReLU
→ Dropout

→ Output Layer
```

---

## 5. Training

The model was trained using:
- CrossEntropyLoss
- Backpropagation
- Optimizers

Training performance was monitored using:
- Training Loss
- Training Accuracy

---

## 6. Experiments

Two experiments were performed:

| Experiment | Optimizer |
|---|---|
| Experiment 1 | Adam |
| Experiment 2 | SGD |

The purpose was to compare optimizer performance.

---

## 7. Evaluation

The model was evaluated on the testing dataset using:
- Test Accuracy
- Test Loss

---

## 8. Visualization

The following graphs were plotted:
- Training Loss Curve
- Training Accuracy Curve

These graphs help analyze model performance during training.

---

# Results

| Model | Accuracy | Loss |
|---|---|---|
| CNN + Adam | ~98% | Low |
| CNN + SGD | ~96-97% | Low |

The Adam optimizer achieved better performance compared to SGD.

---

# Technologies Used

- Python
- PyTorch
- Torchvision
- Matplotlib
- Google Colab

---

# How to Run the Project

1. Open Google Colab
2. Upload the notebook file
3. Run all cells
4. Wait for training to finish
5. View results and graphs

---

# Conclusion

This project demonstrates how CNNs can successfully classify handwritten digits using deep learning techniques.

The experiments showed that optimizer selection affects model accuracy and loss.
