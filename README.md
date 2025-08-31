Retina Disease Risk Detection
Project Description
This project presents a deep learning model designed to automatically detect the risk of retinal disease from fundus images. The model analyzes images to classify a patient as either "No Disease Risk" or "Disease Risk Present". The primary goal is to serve as a preliminary screening tool to assist doctors.

Methodology
This project was developed using the following key steps and techniques:

Data Preparation and Preprocessing: The RFMiD dataset was used for training, with the model learning from the Disease_Risk column. Images were resized to 224x224 pixels and normalized.

Data Augmentation: To improve the model's generalization ability and prevent overfitting, data augmentation techniques such as rotation, shifting, and horizontal flipping were applied to the training data.

Model Architecture: A deep Convolutional Neural Network (CNN) architecture was built from scratch.

Imbalanced Dataset Solution: Class weights were used to address the class imbalance (fewer "No Risk" samples), ensuring the model learned effectively from both classes.

Optimization: The model was trained with the Adam optimizer using a low learning rate (0.0001). Early Stopping was implemented to halt training at the optimal point and prevent overfitting.

Performance Report
The model's performance was evaluated on an independent test dataset.

Class	Precision	Recall	F1-Score	Support
No Risk	0.63	0.61	0.62	134
Risk Present	0.90	0.90	0.90	506
Weighted Avg	0.84	0.84	0.84	640

Export to Sheets
Overall Accuracy: 84.22%

File Structure
retina-disease-risk.ipynb: The Jupyter Notebook containing all the code for the project, from data preparation to model training and evaluation.

retina_disease_risk.h5: The trained and ready-to-use Keras model. Due to its size, this file is stored using Git LFS.

Setup and Usage
Follow these steps to set up and run the project on your local machine:

Install Git LFS:

Bash

git lfs install
Clone the Repository:

Bash

git clone https://github.com/seyid12/Retina-Disease-Risk-Detection.git
Install Required Libraries:

Bash

pip install pandas tensorflow scikit-learn
Run the Notebook:
Launch Jupyter Notebook and open the retina-disease-risk.ipynb file to view and run the code.

Contact
Name: Seyid Yıldız

Email: seyidyildiz416@gmail.com

LinkedIn: https://www.linkedin.com/in/seyid-yıldız-310091349
