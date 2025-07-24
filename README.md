
# 🧠 Alzheimer's Disease Progression Prediction

This project aims to predict the progression of Alzheimer's Disease using a deep learning model trained on MRI scan images. The system classifies brain images into four categories: **Non-Demented**, **Very Mild Demented**, **Mild Demented**, and **Moderate Demented**.

## 📝 Project Overview

- **Domain**: Medical Imaging / Deep Learning
- **Dataset Source**: Kaggle – [Alzheimer’s Dataset (4 Class of Images)](https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images)
- **Model Type**: Convolutional Neural Network (CNN)
- **Framework Used**: TensorFlow / Keras
- **Platform**: Google Colab

## 👩‍💻 Author Info

- **Name**: A. M. Santina Appalo
- **Class**: CSE - D5 - III Year  

## 📁 Dataset Structure

The dataset includes 4 classes:
- `NonDemented`
- `VeryMildDemented`
- `MildDemented`
- `ModerateDemented`

Images are split into `train`, `test`, and `validation` folders.

## 🧪 Installation and Setup

To run the notebook on Google Colab:

1. Install and authenticate the Kaggle API:
   ```python
   !pip install -q kaggle
   from google.colab import files
   files.upload()  # Upload your kaggle.json
   ```

2. Configure Kaggle credentials:
   ```bash
   !mkdir ~/.kaggle
   !cp kaggle.json ~/.kaggle/
   !chmod 600 ~/.kaggle/kaggle.json
   ```

3. Download and unzip dataset:
   ```bash
   !kaggle datasets download -d tourist55/alzheimers-dataset-4-class-of-images
   !unzip alzheimers-dataset-4-class-of-images.zip -d ./data/
   ```

## 🧠 Model Description

The CNN model was designed and trained to process grayscale MRI images. The architecture includes:
- Multiple convolutional and max-pooling layers
- Flatten layer
- Dense layers with dropout
- `softmax` activation for multiclass classification

## 📊 Evaluation Metrics

- **Accuracy**
- **Loss**
- **Confusion Matrix**
- **Classification Report**


## 🖼 Screenshots

Add screenshots of the interface, charts, or results:
```
![Model Accuracy](screenshots/accuracy_plot.png)
![Prediction Sample](screenshots/prediction_sample.png)
```

## 🔮 Future Improvements

- Hyperparameter tuning with learning rate schedulers
- Integration with web-based diagnostic tools
- Real-time MRI scan image prediction

## ⚖️ License

MIT License

Copyright (c) 2025 A. M. Santina Appalo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
