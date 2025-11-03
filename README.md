# ✋ Hand Gesture Recognition using SVM

This project focuses on building a **Hand Gesture Recognition System** using the **Support Vector Machine (SVM)** algorithm. The system can recognize hand gestures captured through images and classify them into predefined gesture categories.

---

## 🚀 Project Overview

The main goal of this project is to develop a reliable model that can accurately detect and classify hand gestures using image data.  
This can be extended to applications such as:
- Human–Computer Interaction  
- Sign Language Recognition  
- Gesture-based Control Systems  
- Virtual Reality Interfaces  

---

## 🧠 Machine Learning Workflow

1. **Data Collection**
   - The dataset used is the **LeapGestRecog** dataset from Kaggle.
   - It contains gesture images of different hand signs taken under various lighting conditions and users.
   - Each gesture is stored in a folder corresponding to its class label.

2. **Data Preprocessing**
   - Converted images to grayscale.
   - Resized all images to a fixed dimension (e.g., 64×64).
   - Flattened the image pixels into feature vectors.
   - Normalized data to improve SVM performance.

3. **Feature Extraction**
   - Used pixel intensity values as input features.
   - Can be extended to use **HOG (Histogram of Oriented Gradients)** features for better performance.

4. **Model Training**
   - Split dataset into **train (80%)** and **test (20%)**.
   - Trained an SVM classifier using `scikit-learn`’s `SVC` with `rbf` and `linear` kernels.
   - Tuned hyperparameters using **GridSearchCV**.

5. **Model Evaluation**
   - Evaluated performance using accuracy, confusion matrix, and classification report.

6. **Gesture Prediction**
   - The trained model can take a new gesture image and predict its corresponding class.

---

## 🧩 Technologies Used

- **Python 3**
- **OpenCV**
- **scikit-learn**
- **NumPy**

---

## 📊 Results

| Kernel | Accuracy | 
|---------|-----------|
| Linear  | 99.92%     | 
| RBF     | 99.5%     | 
| Poly    | 99.87%     | 

The **Linear kernel** provided the highest classification accuracy.
