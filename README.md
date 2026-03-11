# Cotton-Plant-Disease-Detection🌿


Cotton Plant Disease Detection using Deep Learning
📌 Overview

Cotton is one of the most important commercial crops in agriculture. Diseases affecting cotton plants significantly reduce yield and quality, directly impacting farmers' income and agricultural productivity. Early and accurate detection of these diseases can help farmers take preventive measures and reduce crop loss.

Cotton Plant Disease Detection is a deep learning-based computer vision project that identifies diseases in cotton plant leaves using image classification techniques. The model analyzes leaf images and predicts the type of disease affecting the plant.

This project demonstrates how Artificial Intelligence and Deep Learning can assist agriculture by enabling automated disease detection using image data.

🎯 Project Objectives

Detect diseases in cotton plant leaves using image classification.

Build a deep learning model capable of distinguishing between healthy and diseased leaves.

Improve crop monitoring and support early disease diagnosis.

Demonstrate the practical application of AI in agriculture.

🧠 Diseases Detected

The model is trained to classify cotton leaves into the following six categories:

Aphids

Army Worms

Bacterial Blight

Powdery Mildew

Target Spot

Healthy Leaf

Each class represents a specific disease or a healthy cotton leaf.

🗂 Dataset

The dataset consists of images of cotton leaves categorized into six classes.
Images include both healthy leaves and leaves affected by different diseases.

Dataset Details

Image format: JPG/PNG

Image size used for training: 180 × 180 pixels

Classes: 6

Dataset split:

Training set: 80%

Validation set: 20%

🧰 Technologies Used
Technology	Purpose
Python	Programming language
TensorFlow	Deep learning framework
Keras	Neural network API
NumPy	Numerical computations
Matplotlib	Visualization
Pillow	Image processing
🏗 Model Architecture

The project uses a Convolutional Neural Network (CNN) built with TensorFlow and Keras.

Key components of the model:

Image preprocessing and normalization

Convolutional layers for feature extraction

MaxPooling layers to reduce spatial dimensions

Dropout layer to reduce overfitting

Fully connected dense layers for classification

Softmax output layer for predicting disease classes

⚙️ Data Preprocessing

Before training the model, several preprocessing steps were applied:

Image resizing to 180 × 180

Pixel value normalization (scaled to range 0–1)

Dataset batching for efficient training

Data caching and prefetching for performance optimization

🔄 Data Augmentation

To improve model generalization and prevent overfitting, data augmentation techniques were applied:

Random rotation

Horizontal flipping

Zoom transformation

Image shifting

These transformations create multiple variations of existing images, increasing dataset diversity.

📊 Model Training

Training configuration:

Epochs: 10

Batch size: 32

Optimizer: Adam

Loss function: Sparse Categorical Crossentropy

Metrics: Accuracy

📈 Training Results

After applying data augmentation and dropout to reduce overfitting, the model achieved:

Metric	Score
Training Accuracy	~80%
Validation Accuracy	~70%

The gap between training and validation accuracy was reduced, indicating better generalization of the model.

🔍 Prediction Process

The prediction pipeline works as follows:

Input image of a cotton leaf

Image preprocessing and resizing

Model inference using trained CNN

Classification into one of the disease categories

Output predicted disease label

📦 Model Saving

The trained model was saved using TensorFlow’s SavedModel format. This allows the model to be:

Loaded for inference

Deployed using TensorFlow Serving

Integrated into web or mobile applications

🚀 Potential Applications

This project can be extended into several real-world applications:

Mobile application for farmers

AI-powered crop monitoring systems

Smart agriculture platforms

Automated disease detection tools

Precision farming solutions

📁 Project Structure
Cotton-Plant-Disease-Detection/
│
├── README.md
├── ML/
│   ├── models.config
│   └── models/
│       └── cotton_plant_disease_model/
│           └── 1/
│               ├── fingerprint.pb
│               ├── keras_metadata.pb
│               └── variables/
│
└── notebooks/
    └── Cotton_Plant_Disease_Detection.ipynb
💡 Future Improvements

Increase dataset size for better accuracy

Implement transfer learning using pretrained models (ResNet, MobileNet, EfficientNet)

Deploy the model as a web application

Develop a mobile-based disease detection system

Integrate treatment recommendations for detected diseases

👨‍💻 Author

Prathamesh

Full Stack & AI Developer
Specializing in Python, Machine Learning, Data Science, and AI-powered applications.

📜 License

This project is open-source and available for educational and research purposes.

⭐ If you found this project useful, consider giving it a star on GitHub.
