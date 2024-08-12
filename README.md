# Breast Cancer Classification

This repository contains a deep learning-based classification model for predicting breast cancer using a neural network. The model is trained on the Wisconsin Breast Cancer dataset and can classify whether a tumor is malignant or benign based on various features.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model](#model)
- [Results](#results)
- [Streamlit Application](#streamlit-application)
- [Contributing](#contributing)
- [License](#license)

## Overview
Breast cancer is one of the most common cancers among women. Early detection through classification can significantly improve treatment outcomes. This project uses a neural network to classify breast cancer tumors as either malignant or benign based on several features extracted from cell nuclei present in digitized images of a fine needle aspirate (FNA) of a breast mass.

## Features
- **Deep Learning Model**: A neural network trained for high accuracy classification.
- **Preprocessing**: Data is scaled using a pre-trained scaler to improve model performance.
- **Streamlit Web App**: An interactive web application built with Streamlit to allow users to input features and get predictions.

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/alihassanml/Breast-Cancer-Classification.git
   cd Breast-Cancer-Classification
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Make sure the following files are in the project directory:
   - `model.h5`: The pre-trained neural network model.
   - `scalar.pkl`: The scaler used for feature scaling.

## Usage
### Running the Streamlit App
You can run the Streamlit app to make predictions using the trained model:

```bash
streamlit run app.py
```

### Input Features
The app requires the following features to make a prediction:

- Mean Radius
- Mean Texture
- Mean Perimeter
- Mean Area
- Mean Smoothness
- Mean Compactness
- Mean Concavity
- Mean Concave Points
- Mean Symmetry
- Mean Fractal Dimension
- Radius Error
- Texture Error
- Perimeter Error
- Area Error
- Smoothness Error
- Compactness Error
- Concavity Error
- Concave Points Error
- Symmetry Error
- Fractal Dimension Error
- Worst Radius
- Worst Texture
- Worst Perimeter
- Worst Area
- Worst Smoothness
- Worst Compactness
- Worst Concavity
- Worst Concave Points
- Worst Symmetry
- Worst Fractal Dimension

### Model Prediction
The model outputs a prediction indicating whether the tumor is likely to be malignant or benign.

## Model
The neural network model is built using TensorFlow and Keras. It has been trained on the Wisconsin Breast Cancer dataset, achieving an accuracy of 98.40% on the test set.

## Results
### Confusion Matrix:
```
[[ 66   1]
 [  2 119]]
```

### Classification Report:
```
              precision    recall  f1-score   support

           0       0.97      0.99      0.98        67
           1       0.99      0.98      0.99       121

    accuracy                           0.98       188
   macro avg       0.98      0.98      0.98       188
weighted avg       0.98      0.98      0.98       188
```

## Streamlit Application
The Streamlit application provides a user-friendly interface to input the necessary features and receive a prediction. The app is designed for easy deployment and use.

## Contributing
Contributions are welcome! If you have any suggestions, feel free to open an issue or create a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
