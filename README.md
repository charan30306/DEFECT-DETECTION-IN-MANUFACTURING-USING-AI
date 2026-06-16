# DEFECT-DETECTION-IN-MANUFACTURING-USING-AI
## Overview
This project implements an automated defect detection system for industrial casting products using Deep Learning and Transfer Learning. A pre-trained MobileNetV2 model is fine-tuned to classify casting images as either defective or non-defective, enabling efficient quality inspection in manufacturing environments.

## Features
- Automated defect detection from casting images
- Transfer Learning using MobileNetV2
- Fine-tuning for improved classification performance
- Data augmentation and preprocessing
- Model evaluation using classification metrics
- Confusion matrix visualization
- Model saving and deployment-ready export

## Dataset
The project uses the Real-Life Industrial Dataset of Casting Products available on Kaggle.

Dataset Link:
https://www.kaggle.com/datasets/ravirajsinh45/real-life-industrial-dataset-of-casting-product

### Classes
- Defective Casting (def_front)
- Non-Defective Casting (ok_front)

## Technologies Used
- Python
- TensorFlow / Keras
- MobileNetV2
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- OpenCV

## Project Workflow
1. Load and preprocess casting images
2. Split data into training, validation, and testing sets
3. Apply data augmentation
4. Build the MobileNetV2 transfer learning model
5. Train the classification model
6. Fine-tune the top layers of MobileNetV2
7. Evaluate model performance
8. Save the trained model for future use

## Model Architecture
- Base Model: MobileNetV2 (ImageNet Weights)
- Global Average Pooling Layer
- Batch Normalization Layer
- Dense Layers with Dropout
- Sigmoid Output Layer for Binary Classification

## Evaluation Metrics
The model is evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## Results
The trained model successfully classifies casting products into defective and non-defective categories, demonstrating the effectiveness of transfer learning for industrial quality inspection tasks.

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/defect-detection-casting.git
cd defect-detection-casting
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the Project

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run all cells in:

```text
defect_detection_manufacturing.ipynb
```

## Saved Model

The trained model is stored as:

```text
defect_detection_model.keras
```

## Future Improvements
- Real-time defect detection using webcam/video streams
- Deployment using Flask or FastAPI
- Explainable AI with Grad-CAM
- Multi-class defect classification
- Integration with industrial inspection systems

## Author
Charan Reddy Padala
