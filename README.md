Handwritten Digit Recognition

A machine learning project that recognizes handwritten digits (0–9) using a Convolutional Neural Network (CNN).

This project explores deep learning and computer vision by training a model to classify handwritten digit images and making it accessible through an interactive web application.

Technologies Used

- Python
- TensorFlow / Keras
- Convolutional Neural Networks (CNN)
- NumPy
- Gradio
- Pillow (PIL)

Dataset

The model was trained using the MNIST handwritten digit dataset, which contains:

- 60,000 training images
- 10,000 testing images
- 28 × 28 grayscale images
- 10 digit classes (0–9)

Model Architecture

The project uses a Convolutional Neural Network (CNN) designed for image classification.

The architecture consists of:

1. First convolutional layer with 32 filters and ReLU activation.
2. Max pooling layer.
3. Second convolutional layer with 64 filters and ReLU activation.
4. Max pooling layer.
5. Flatten layer.
6. Fully connected Dense layer with 128 neurons and ReLU activation.
7. Dropout layer with a rate of 0.3 to help reduce overfitting.
8. Output layer with 10 neurons and Softmax activation.

Training Configuration

- Optimizer: Adam
- Loss function: Sparse Categorical Crossentropy
- Early stopping to monitor validation loss and restore the best model weights.

Model Performance

The trained model achieved a test accuracy of 99.17% on the MNIST test dataset.

This demonstrates the model's ability to classify handwritten digits accurately on the test images.

Interactive Demo

The project includes an interactive web application built with Gradio, allowing users to draw handwritten digits and receive predictions from the trained model.

Users can also view the model's top three predicted classes.

Live Demo

[Try the Handwritten Digit Recognizer](https://capstone-project-88mw.onrender.com)

Project Files

- "app.py" – Gradio application.
- "requirement.txt" – Project dependencies.
- "CNN_2.ipynb" – Jupyter Notebook containing the model development and training workflow.
- "CNN_model (1).h5" – Saved trained CNN model.

Future Improvements

- Improve prediction consistency across different handwriting styles.
- Explore model optimization and deployment improvements.
- Expand the application with additional features.
