📌 Emotion Detection using CNN & OpenCV
📖 Overview

This project is a Real-Time Emotion Detection System that uses Deep Learning (CNN) and OpenCV to detect human emotions from facial expressions via webcam.

The model is trained on grayscale facial images and can classify emotions into multiple categories.

🎯 Features
Real-time face detection using Haar Cascade
Emotion classification using CNN
Live webcam prediction
Training + validation visualization (accuracy & loss graphs)
Supports 7 emotion classes
🧠 Model Performance
📊 Training vs Validation Accuracy & Loss

👉 From your results:

Training accuracy increases up to ~87%
Validation accuracy stabilizes around ~62%
Validation loss increases after some epochs → overfitting observed
🗂️ Project Structure
├── data/
│   ├── train/
│   └── test/
├── kerasmodel.py
├── model.h5
├── haarcascade_frontalface_default.xml
├── plot.png
├── manage.py
└── README.md
⚙️ Technologies Used
Python
TensorFlow / Keras
OpenCV
NumPy
Matplotlib
Django (for backend)
🚀 Installation
git clone 
cd emotion-detection
pip install -r requirements.txt
▶️ How to Run
🔹 Train the Model
python kerasmodel.py --mode train
🔹 Run Real-Time Detection
python kerasmodel.py --mode display
🧩 How It Works
Face Detection
Uses Haar Cascade classifier
File:

Model Architecture

Multiple Conv2D + MaxPooling layers
Dense layers for classification
Dropout for regularization

(See implementation in )

Prediction
Captures webcam frames
Detects face
Predicts emotion
😊 Emotion Classes
Angry
Disgusted
Fearful
Happy
Neutral
Sad
Surprised

📉 Limitations
Overfitting observed in validation results
Performance depends on lighting conditions
Works best with frontal face


👨‍💻 Author

Mahesh K
