🩻 AI-Powered Pneumonia Detection

A Deep Learning application that detects Pneumonia from chest X-Ray images using a Convolutional Neural Network (CNN). This tool assists biomedical engineers and radiologists by flagging high-probability scans for review.

🚀 Features

Deep Learning Architecture: Uses a custom CNN optimized for grayscale medical imaging.

Data Augmentation: Implements zoom, shear, and flip operations to prevent overfitting.

High Accuracy: Targets >90% accuracy on the test set.

Fast Inference: Can process a single X-ray image in under 200ms.

📂 Dataset

This project uses the Chest X-Ray Images (Pneumonia) dataset.

Download it from Kaggle.

Extract it into a folder named dataset/ in this directory.

Your folder structure should look like this:

/dataset
   /train
       /NORMAL
       /PNEUMONIA
   /test
       /NORMAL
       /PNEUMONIA


🛠️ Installation

Clone the repository.

Install dependencies:

pip install -r requirements.txt


🧠 Training the Model

Run the training script to build the neural network and start learning:

python train.py


The model will save automatically as pneumonia_model.h5.

Training logs will show accuracy improving over "epochs".

🩺 Running a Diagnosis (Inference)

To check a specific X-ray image:

python predict.py --image path/to/patient_scan.jpeg


📊 Tech Stack

Language: Python 3.9+

Framework: TensorFlow / Keras

Image Processing: OpenCV, NumPy
