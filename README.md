# Blood-Cell-Image-Classification
Overview This project focuses on the classification of blood cell images into four categories: Eosinophil, Lymphocyte, Monocyte, and Neutrophil. The goal is to automate the identification and characterization of blood cell subtypes, which has important applications in medical diagnostics.


Dataset
Source: BCCD Dataset
Description:
The dataset contains 12,500 augmented images of blood cells (JPEG format) with corresponding cell type labels. There are approximately 3,000 images for each of the four cell types, grouped into separate folders. The dataset is split into training and test sets, each containing images of all four classes.
Classes:
Eosinophil
Lymphocyte
Monocyte
Neutrophil
Project Workflow
Data Preparation
Images are resized to 64x64 pixels.
Normalization is applied using ImageNet statistics.
Data is loaded using PyTorch's ImageFolder and DataLoader.
Model Architecture
A custom Convolutional Neural Network (CNN) is implemented using PyTorch.
The architecture consists of several convolutional and pooling layers, followed by fully connected layers and dropout for regularization.
Training
The model is trained using the Adam optimizer and CrossEntropyLoss.
Training and validation losses are tracked and visualized to monitor overfitting.
Evaluation
The trained model is evaluated on the test set.
Metrics such as accuracy, F1 score, and ROC AUC are calculated and reported.
Results
Test Accuracy: ~0.86
Test F1 Score: ~0.86
Test ROC AUC: ~0.97
The model demonstrates strong performance in classifying blood cell images and can be further improved with more advanced architectures or data augmentation techniques.
метрики говорят о том, что модель обучена хорошо и обобщает на тесте. Ты всё сделал правильно!
