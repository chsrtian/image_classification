# 🧥 Image Classification with Fashion MNIST

A neural network project that classifies clothing items using the Fashion MNIST dataset.

📓 **[View the Google Colab Notebook](https://colab.research.google.com/drive/1B_nARTmBezqlWirrarYKWsb_WjlqXuoM?usp=sharing)**

---

## 📋 Table of Contents

- [About the Dataset](#about-the-dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Architecture](#model-architecture)
- [Training Process](#training-process)
- [Results](#results)
- [Improving Accuracy](#improving-accuracy)

---

## About the Dataset

### What is the Fashion MNIST dataset?

Based on my experiment, the Fashion MNIST dataset is a collection of grayscale images used for training and testing an image classification model. Each image has a resolution of **28×28 pixels** and represents different clothing items such as:

- Shirts
- Shoes
- Trousers
- Bags

I used this dataset to observe how well a neural network can classify clothing images. Compared to the original MNIST dataset, Fashion MNIST is more challenging because it contains more complex and realistic image patterns.

---

## Data Preprocessing

### Why do we normalize image pixel values before training?

In my observation, We normalized the image pixel values by dividing them by **255** so that all values are within the range of **0 to 1**. This helped make the training process more stable and faster.

Normalization allowed the model to:
- Update its weights more efficiently
- Prevent large pixel values from negatively affecting the learning process

---

## Model Architecture

### Layers used in the neural network

| Layer | Function |
|-------|----------|
| **Flatten** | Converts the 28×28 image into a one-dimensional array so it can be processed by the neural network |
| **Dense (Hidden)** | Uses ReLU activation to learn important features from the images |
| **Dense (Output)** | Contains 10 neurons corresponding to the 10 clothing categories in the Fashion MNIST dataset |


---

## Training Process

### What does an epoch mean in model training?

An **epoch** refers to one complete pass of the entire training dataset through the model.

In my experiment, training the model for several epochs allowed it to:
- Gradually improve its accuracy
- Reduce its loss

By observing the changes in accuracy per epoch, I was able to see how the model learned over time.

---

## Results

### Comparing predicted and actual labels

Based on my results, the **predicted label** for the first test image matched the **actual label** provided in the dataset.

This indicates that:
- The model was able to correctly classify the image
- The model learned useful patterns from the training data

Comparing the predicted and actual labels helped me evaluate the model's performance on unseen data.

---

## Improving Accuracy

### What could be done to improve the model's accuracy?

Based on my experiment, increasing the number of hidden layers slightly improved the model's accuracy.

| Model Configuration | Test Accuracy |
|---------------------|---------------|
| One hidden layer | **0.8917** |
| Two hidden layers | **0.8935** |

This indicates that adding another hidden layer allowed the model to learn additional features from the dataset, resulting in a small improvement in performance.

However, the improvement was minimal, which suggests that simply adding more layers does not always lead to a significant increase in accuracy.


