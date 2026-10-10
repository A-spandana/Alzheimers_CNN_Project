# Alzheimers_CNN_Project
Alzheimer's Disease Detection using CNN.
# Alzheimer’s Disease Detection Using Convolutional Neural Network (CNN)

## 1. Project Overview

This project aims to classify Alzheimer’s disease stages from brain MRI images using a Convolutional Neural Network (CNN). Deep learning techniques are used to learn image features and classify MRI scans into four categories.

The project is developed using Python and TensorFlow in Google Colab.

## 2. Problem Statement

Alzheimer’s disease is a progressive neurological disorder that affects memory and cognitive abilities. Analyzing MRI images can help researchers study brain changes associated with the disease. This project explores the use of a CNN to classify MRI images into different categories.

**Note:** This is an educational research project and is not intended for clinical diagnosis.

## 3. Objectives

- Develop a CNN model for classifying Alzheimer’s MRI images.
- Preprocess and normalize MRI images before training.
- Train and validate the model using a labeled dataset.
- Evaluate performance using accuracy, precision, recall, F1-score, and a confusion matrix.

## 4. Dataset

The project uses the **Alzheimer MRI Dataset** obtained from Kaggle.

The dataset contains MRI images organized into four classes:

- NonDemented
- VeryMildDemented
- MildDemented
- ModerateDemented

**Dataset source:** [https://www.kaggle.com/datasets/azminur2856/alzheimer-mri-dataset]

The dataset is divided into training and validation subsets. Image files are loaded from class-specific folders.

## 5. Technologies Used

- Python
- Google Colab
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn

## 6. Methodology

### Data Preprocessing
- Load MRI images from the dataset folders.
- Resize images to 128 × 128 pixels.
- Create training and validation datasets.
- Normalize pixel values to the range 0–1.

### CNN Model Development

The CNN model consists of convolutional layers, max-pooling layers, a flattening layer, dense layers, and a dropout layer. The output layer uses softmax activation to predict one of the four classes.

### Model Training

The model is compiled using the Adam optimizer and sparse categorical cross-entropy loss. Early stopping and model checkpointing are used during training.

### Model Evaluation

The model is evaluated using validation loss, accuracy, precision, recall, F1-score, and a confusion matrix.

## 7. Project Structure

```text
Alzheimers_CNN_Project/
├── Alzheimers_CNN_Project.ipynb
├── README.md
├── requirements.txt
├── Project_Report.docx
├── results/
│   ├── confusion_matrix.csv
│   ├── classification_report.txt
│   └── training_history.json
└── data/
    └── README.md
```

## 8. Requirements

Install the required libraries using:

```bash
pip install -r requirements.txt
```

The `requirements.txt` file should list the required Python packages, such as TensorFlow, NumPy, Matplotlib, and Scikit-learn.

## 9. How to Run the Project

1. Download or clone this repository.
2. Open `Alzheimers_CNN_Project.ipynb` in Google Colab or Jupyter Notebook.
3. Obtain the dataset from the source listed above.
4. Upload or configure the dataset path as required by the notebook.
5. Run the notebook cells in order to preprocess the images, train the CNN model, and evaluate its performance.

## 10. Results

The model is evaluated using validation accuracy, precision, recall, F1-score, and a confusion matrix.

**Actual validation accuracy:** [Validation Accuracy: 89.06%]

**Other evaluation results:** Refer to the classification report and confusion matrix included in the `results/` folder.

## 11. Limitations

- The model's performance depends on the quality and distribution of the dataset.
- Validation results do not guarantee performance on images from other datasets or clinical settings.
- MRI image classification alone cannot establish a medical diagnosis.
- Further testing on independent datasets is needed.

## 12. Future Scope

- Evaluate the model using independent MRI datasets.
- Explore data augmentation and alternative CNN architectures.
- Investigate model interpretability techniques such as Grad-CAM.
- Study generalization across different imaging sources.

## 13. References

1. The original Kaggle dataset page used for this project.
2. TensorFlow documentation: https://www.tensorflow.org/
3. Scikit-learn documentation: https://scikit-learn.org/stable/

