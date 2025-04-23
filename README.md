# 😊 Face Emotional Recognition

A deep learning project for detecting human emotions from facial expressions using Convolutional Neural Networks (CNN) and TensorFlow/Keras. The model can recognize multiple emotions such as, **happy**, **sad**, and **neutral**.

## 📌 Overview

This project aims to build a robust image classification model that can detect facial emotions from images. The dataset is pre-organized into training, validation, and testing sets. The final model is also exported to TensorFlow.js format for web deployment.

## 🗂️ Dataset Structure

The dataset directory is structured as follows:

dataset/ ├── train/ │ ├── happy/ │ ├── sad/ │ └── neutral/ ├── val/ │ └── ... └── test/ └── ...


Each folder contains facial images labeled by emotion.

## 🧠 Model Architecture

- Input: 224x224 RGB images
- Layers:
  - Convolution + ReLU
  - MaxPooling
  - BatchNormalization
  - Dense layers
  - Dropout
- Output: Softmax layer (multi-class classification)

## 🔧 Features

- Image preprocessing and augmentation using `ImageDataGenerator`
- Categorical classification using softmax
- Evaluation with confusion matrix and classification report
- Training history visualization
- Model export to TensorFlow.js (`.json` and `.bin` format)

## 📈 Results

- Trained model shows strong accuracy across emotion classes
- Includes plots of training/validation accuracy and loss
- Confusion matrix to visualize prediction performance

## 📦 Installation

Install the required dependencies:

```pip install tensorflow keras tensorflowjs matplotlib pandas pillow scikit-learn```

Or generate the full list with:

```pip install pipreqs```
```pipreqs /path/to/project --force --ignore some_file.ipynb --scan-notebooks```

⚠️ Use !pipreqs in Jupyter Notebook instead of pipreqs to avoid SyntaxError.

🌐 Web Deployment
Convert the Keras model to TensorFlow.js format:

```tensorflowjs_converter --input_format keras model.h5 tfjs_model/```

Place tfjs_model/ into your web app directory and load with TensorFlow.js in the browser.

📊 Visualizations

- 📉 Accuracy & Loss plot

- 📊 Confusion matrix for evaluation

📚 References
- TensorFlow Documentation

- Keras API Reference

- TensorFlow.js

✨ License
MIT License — feel free to use, modify, and share.

🤝 Acknowledgements
This project is part of an academic exploration into computer vision and emotion recognition using deep learning.
