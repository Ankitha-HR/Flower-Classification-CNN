# Flower Classification Using Convolutional Neural Network (CNN)

## Project Overview
This project uses Deep Learning and Convolutional Neural Networks (CNNs) to classify flower images into five categories. It uses TensorFlow and Keras to build, train, and evaluate image classification models.

## Objective
To develop a CNN model that can identify the category of a flower from an input image and display the predicted class with its confidence score.

## Dataset
- **Dataset:** TensorFlow Flower Photos dataset
- **Source:** [TensorFlow Flower Photos](https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz)
- **Categories:** Daisy, Dandelion, Roses, Sunflowers, and Tulips
- **Image size:** 180 × 180 pixels
- **Training split:** 80%
- **Validation split:** 20%

The dataset is downloaded automatically by the notebook.

## Technologies Used
- Python
- Google Colab
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Seaborn

## Methodology

### 1. Data Preparation
- Download and load the flower image dataset.
- Identify the five flower categories.
- Resize images to 180 × 180 pixels.
- Split the dataset into training and validation sets.
- Normalize image pixel values to the range 0–1.

### 2. CNN Model 1
The first CNN model contains:
- Convolutional layers with 16, 32, and 64 filters.
- Max-pooling layers.
- A flattening layer.
- A dense layer with 128 neurons.
- An output layer for five flower classes.

The model uses the Adam optimizer and sparse categorical cross-entropy loss.

### 3. Improved CNN Model
The second model improves training using:
- Random horizontal flipping.
- Random image rotation.
- Random zoom.
- Dropout regularization to help reduce overfitting.

The improved model is trained for 15 epochs.

### 4. Model Evaluation
The notebook evaluates the model using:
- Training accuracy and loss.
- Validation accuracy and loss.
- Confusion matrix.
- Precision, recall, and F1-score for each class.

### 5. Flower Image Prediction
A user can upload a flower image. The trained model predicts its flower category and displays the prediction confidence.

## Workflow
1. Download the dataset.
2. Explore flower categories and sample images.
3. Preprocess and split the dataset.
4. Build and train the first CNN model.
5. Improve the model using data augmentation and dropout.
6. Evaluate the model using classification metrics.
7. Upload a flower image and predict its category.

## How to Run
1. Open the notebook in Google Colab.
2. Run the cells in order.
3. Allow the dataset to download.
4. Train the CNN models.
5. Review the evaluation plots and classification report.
6. Upload a flower image in the prediction section to test the model.

## Results
The notebook compares the initial CNN model with an improved CNN model using data augmentation and dropout. It also generates accuracy and loss plots, a confusion matrix, and a classification report.

**Note:** Actual validation accuracy and other metric values should be added after running the notebook and confirming the results.

## Conclusion
This project demonstrates how CNNs can be used for flower image classification. It covers image preprocessing, model training, data augmentation, performance evaluation, and prediction on new images using TensorFlow and Keras.

## Repository Contents
- `Flower_Classification_CNN (2).ipynb` — Jupyter notebook containing the implementation, training, evaluation, and prediction workflow.

## Future Enhancements
- Improve accuracy through hyperparameter tuning.
- Compare the CNN with transfer-learning models such as MobileNetV2.
- Develop a simple web interface for uploading and classifying flower images.
