# Industrial-Surface-Crack-Detection-using-CNN-Project-
Industrial Surface Crack Detection using CNN is a deep learning-based image classification project designed to automatically detect cracks on industrial surfaces. The project uses a Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify surface images into two categories: Crack and No Crack. The system performs dataset preparation, image preprocessing, augmentation, CNN model training, validation, testing, performance evaluation, model saving, and single-image prediction.

Key Features
Dataset Validation: Checks whether the Positive and Negative image folders exist and contain valid image files.
Dataset Organization: Automatically creates separate folders for training, validation, and testing with Crack and NoCrack classes.
Data Splitting: Divides the dataset into approximately 70% training, 15% validation, and 15% testing data.
Image Preprocessing: Resizes images to 128 × 128 pixels and normalizes pixel values from 0–255 to approximately 0–1.
Data Augmentation: Applies rotation, zoom, width/height shifting, and horizontal flipping to training images to improve model generalization.
CNN Architecture: Uses multiple convolutional layers with 32, 64, 128, and 256 filters, followed by batch normalization and max-pooling layers to extract important visual features.
Classification: Uses fully connected Dense layers and a final sigmoid output layer for binary Crack/No Crack classification.
Overfitting Control: Uses Dropout layers with rates of 0.5 and 0.3 to reduce overfitting.
Training Optimization: Uses the Adam optimizer and binary cross-entropy loss for model training.
Training Callbacks: Implements Early Stopping, Model Checkpointing, and Reduce Learning Rate on Plateau to improve training efficiency and preserve the best model.
Performance Evaluation: Evaluates the model on unseen test data using test accuracy, confusion matrix, and classification report.
Visualization: Generates training/validation accuracy and loss graphs to monitor model performance.
Single Image Prediction: Allows an individual surface image to be supplied to the trained model and returns "Crack Detected" or "No Crack".
Model Saving: Saves both the best checkpoint and final trained CNN model in .keras format.
Technologies Used

Python, TensorFlow, Keras, NumPy, Matplotlib, Scikit-learn, CNN, Image Processing, Deep Learning

Project Workflow

Dataset → Validation → Train/Validation/Test Split → Image Preprocessing → Data Augmentation → CNN Model Building → Model Training → Validation → Performance Evaluation → Model Saving → Single Image Prediction
