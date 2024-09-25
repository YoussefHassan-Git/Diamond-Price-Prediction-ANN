# 💎 Diamond Price Prediction using Artificial Neural Network (ANN)

This project aims to predict the price of diamonds based on various features such as carat, cut, color, clarity, and more. Using a dataset of diamond features, we build an Artificial Neural Network (ANN) to predict the prices accurately.

## 📚 Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Model Performance](#model-performance)
- [Graph](#graph)

---

## 🛠️ Project Overview

- The goal of this project is to develop an ANN model that can predict the price of a diamond based on its features such as carat, cut, color, clarity, and more.
  
- The model is built using the **TensorFlow** and **Keras** libraries.

---

## 📁 Dataset

- The dataset used in this project is the **Diamond Prices** dataset, which includes features like:
  - **Carat**: The weight of the diamond.
  - **Cut**: Quality of the cut (Fair, Good, Very Good, Premium, Ideal).
  - **Color**: Diamond color grading.
  - **Clarity**: Clarity of the diamond (I1, SI1, VS2, etc.).
  - **Other features** such as depth, table, and price.

---

## ⚙️ Data Preprocessing

- The dataset is cleaned and preprocessed before being fed into the model. Key preprocessing steps include:
  - **One-Hot Encoding**: Applied to categorical features such as cut, color, and clarity.
  - **Min-Max Scaling**: Applied to numerical features to bring them into the range [0,1].
  - **Train-Test Split**: The dataset is split into training and testing sets.

---

## 🏗️ Model Architecture

The ANN model is built using **Keras Sequential API** with the following layers:

```python
model = tf.keras.Sequential([
    tf.keras.layers.Dense(300),    
    tf.keras.layers.Dense(128),
    tf.keras.layers.Dense(64),
    tf.keras.layers.Dense(64),
    tf.keras.layers.Dense(32),

    # Output layer (Dense)
    model.add(Dense(1, activation='linear'))  # For regression tasks
])


```
---

## 🎓 Training
The model is compiled using the Adam optimizer and MAE as the loss function.
The model is trained for 200 epochs with an early stopping mechanism to avoid overfitting.
---
## 📈 Model Performance

`Mae: 648.5654`
---
## Graph
![download](https://github.com/user-attachments/assets/94d05c6e-2e02-44d9-bd78-18c09deb35ee)


