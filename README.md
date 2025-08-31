# Retina Disease Risk Detection

## Project Description
This project presents a deep learning model designed to automatically detect the risk of retinal disease from fundus images. The model analyzes images to classify a patient as either **"No Disease Risk"** or **"Disease Risk Present"**. The primary goal is to serve as a preliminary screening tool to assist doctors.

## Methodology
This project was developed using the following key steps and techniques:

- **Data Preparation and Preprocessing:** The RFMiD dataset was used for training, with the model learning from the `Disease_Risk` column. Images were resized to 224x224 pixels and normalized.
- **Data Augmentation:** Techniques such as rotation, shifting, and horizontal flipping were applied to the training data to improve generalization and prevent overfitting.
- **Model Architecture:** A deep Convolutional Neural Network (CNN) was built from scratch.
- **Imbalanced Dataset Solution:** Class weights were used to address the class imbalance (fewer "No Risk" samples), ensuring the model learned effectively from both classes.
- **Optimization:** The model was trained with the Adam optimizer using a low learning rate (0.0001). Early Stopping was implemented to halt training at the optimal point.

## Performance Report
The model's performance was evaluated on an independent test dataset:

| Class      | Precision | Recall | F1-Score | Support |
|------------|-----------|--------|----------|--------|
| No Risk    | 0.63      | 0.61   | 0.62     | 134    |
| Risk Present | 0.90    | 0.90   | 0.90     | 506    |
| **Weighted Avg** | 0.84 | 0.84   | 0.84     | 640    |

**Overall Accuracy:** 84.22%

## File Structure
- `retina-disease-risk.ipynb`: Jupyter Notebook containing all the code for data preparation, model training, and evaluation.
- `retina_disease_risk.h5`: Trained Keras model (stored using Git LFS due to its size).

## Setup and Usage
1. **Install Git LFS:**

Clone the Repository:

git clone https://github.com/seyid12/Retina-Disease-Risk-Detection.git


Install Required Libraries:

pip install pandas tensorflow scikit-learn


Run the Notebook:
Launch Jupyter Notebook and open retina-disease-risk.ipynb to view and run the code.

Contact

Name: Seyid Yıldız

Email: seyidyildiz416@gmail.com

LinkedIn: https://www.linkedin.com/in/seyid-yıldız-310091349



```bash
git lfs install
