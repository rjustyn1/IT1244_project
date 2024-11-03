# IT1244 Project
## Description

In recent years there has been interest in develping Convolutional Neural Network (CNN) machine learning models that can assist in classifying MRI scans of brain tumors into benign or malignant. Our project aims to build on previous works by experimenting with the application of GradCAM to visualise the decision making done by CNNs as well as exploring different ways to augment our training data to allow the trained model to be more robust and flexible.

## Workflow
The workflow is as follows:

- Data Preparation which consists of two steps:
  - Preprocessing
  - Augmentation
- Training and analysing the baseline CNN model which consists of:
  - (Training) Creation of model and fine-tuning for optimal hyperparameters
  - (Analysis) Plotting the performance graphs with various metrics used
  - (Analysis) Using GradCAM to visualise model
- Training and analysingthe VGG16-ANN model which consists of:
  - (Training) Creation of multiple models with varied number of VGG16's layers frozen (transfer learning)
  - (Analysis) Plotting the performance graphs with various metrics used
  - (Analysis) Using GradCAM to visualise model
- Training and analysing the CNN-XGBoost model which consists of:
  - (Training) Creation of model and incorporation of Principal Component Analysis (PCA) into model as well as hyperparameter tuning
  - (Analysis) Plotting the performance graphs with various metrics used
  - # Note : As this model depend heavily on XGBoost as the classifier, the convolution layers in the CNN solely works as a feature extractor, thus making analytics using GradCAM is not effective.
 

