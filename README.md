CIFAR-10 Image Classification using DNN, CNN, and CNN with Data Augmentation

📌 Project Overview

This project focuses on image classification using the CIFAR-10 dataset and compares the performance of:

Deep Neural Network (DNN)
Convolutional Neural Network (CNN)
CNN with Image Augmentation

The goal of this project is to understand how CNNs outperform traditional DNNs in computer vision tasks by preserving spatial features from images.

📂 Dataset Information
The CIFAR-10 dataset contains:
60,000 color images


Image size: 32 × 32


10 classes:


Airplane


Car


Bird


Cat


Deer


Dog


Frog


Horse


Ship


Truck




Dataset Source:
CIFAR-10 Dataset

🧠 Technologies Used


Python


TensorFlow / Keras


NumPy


Matplotlib


Seaborn


Scikit-learn



🔥 Project Workflow
1️⃣ Data Preprocessing


Loaded CIFAR-10 dataset


Normalized pixel values (0–255 → 0–1)


Applied one-hot encoding to labels


Split dataset into training and validation sets



2️⃣ Deep Neural Network (DNN)
Implemented a fully connected neural network using:


Flatten layer


Dense layers


ReLU activation


Softmax output layer


📊 DNN Result


Test Accuracy: ~43%


❌ Observation
The DNN model struggled because flattening the image removed important spatial relationships between pixels.

3️⃣ Convolutional Neural Network (CNN)
Implemented CNN architecture using:


Conv2D layers


MaxPooling2D


Batch Normalization


Dropout layers


Dense layers


📊 CNN Result


Test Accuracy: ~83%


✅ Observation
CNN significantly outperformed DNN because convolutional layers preserved spatial information and learned important image features such as edges, textures, and shapes.

4️⃣ CNN with Image Augmentation
Applied Image Augmentation using:


Rotation


Width shifting


Height shifting


Horizontal flipping


📊 CNN + Augmentation Result


Test Accuracy: ~80.6%


✅ Observation
Image augmentation improved model robustness and generalization by exposing the model to transformed image variations. Although a slight decrease in accuracy was observed, the model became less dependent on fixed image orientations.

📈 Model Comparison
ModelTest Accuracy
DNN~43%
CNN~83%
CNN + Augmentation~80.6%

🧠 Key Learnings


CNNs are highly effective for image-related tasks.


Spatial feature preservation is critical in computer vision.


DNNs lose image structure after flattening.


Data augmentation improves generalization and robustness.


Confusion matrices help analyze class-wise prediction errors.



📊 Visualization & Evaluation
The project also includes:


Accuracy and Loss Graphs


Prediction Visualization


Confusion Matrix Analysis


Class-wise Error Analysis



🚀 Future Improvements


Transfer Learning using pre-trained models


Hyperparameter tuning


Early stopping and learning rate scheduling


Advanced augmentation techniques


Model deployment using Flask or Streamlit



📁 Project Structure
CIFAR10-Image-Classification/│├── DNN_CIFAR10.ipynb├── CNN_CIFAR10.ipynb├── CNN_Augmented_CIFAR10.ipynb├── README.md│└── saved_models/    ├── dnn_model.h5    ├── cnn_model.h5    └── cnn_augmented_model.h5

💬 Conclusion
This project demonstrates the practical difference between DNNs and CNNs for image classification tasks. Through experimentation and comparison, it highlights why CNNs are the preferred choice for computer vision applications and how augmentation techniques help improve model generalization.

👩‍💻 Author
Prakriti Anand
Machine Learning | AI/ML | Deep Learning Enthusiast
