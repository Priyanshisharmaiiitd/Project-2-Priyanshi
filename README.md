# Project-2-Priyanshi
A deep learning-based retinal blood vessel segmentation system using the U-Net architecture, trained on the DRIVE dataset. The model identifies and highlights blood vessels in fundus images to support early diagnosis of eye diseases like diabetic retinopathy.

# What is Retinal Segmentation?
Retinal vessel segmentation means identifying the blood vessels in eye images (called fundus images) — it's used to detect diseases like:
Diabetic Retinopathy
Glaucoma
Hypertension
The model learns to highlight vessels in green (or white) pixels and ignore the background — a pixel-wise classification problem, aka semantic segmentation.

# What This Project Does
This project uses a U-Net architecture to:
Train a deep learning model on eye images (from the DRIVE dataset)
Predict blood vessel areas on test images
Visualize segmented output images (vessels vs. non-vessels)

# Explanation of Files in Your Folder:-
data.py	-Loads and preprocesses retina images and masks from the dataset
eval.py	-Contains code to evaluate model performance (Dice score, accuracy)
metrics.py-	Custom metric functions like Dice coefficient, precision, recall
model.py-	Defines the U-Net model architecture
train.py-	Trains the model on DRIVE dataset, handles training loop
README.md-	Placeholder ReadMe (you'll replace it with the one I made for you)
results/-	Folder to save segmented output masks (predictions)
new_data/-	May contain your own test images for trying new predictions

# 🧠 Retina Blood Vessel Segmentation using U-Net

This project implements a U-Net deep learning model to segment blood vessels in retina images using the **DRIVE dataset**. The goal is to help early detection of eye diseases like **diabetic retinopathy** through semantic segmentation.

---

## 💻 Technologies Used

- Python
- TensorFlow / Keras
- OpenCV, NumPy, Matplotlib
- U-Net Architecture
- Semantic Segmentation

---

## 📁 Folder Structure
├── train.py # Model training
├── predict.py # Predict segmented masks
├── unet.py # U-Net architecture
├── data.py # Image loading & preprocessing
├── requirements.txt
├── output/ # Predicted mask results


---

## 📊 Dataset

- Dataset: [DRIVE – Retinal Images](https://www.kaggle.com/datasets/andrewmvd/drive-digital-retinal-images-for-vessel-extraction)
- Format: 20 training & 20 test images + masks

Place dataset inside a folder named `drive/`.

---

## 🚀 How to Run

### 1. Install Requirements
```bash
pip install -r requirements.txt
#train model:-
python train.py
#predict:-
python predict.py

📈 Highlights
Achieved ~85% Dice coefficient
Optimized for fast training and evaluation
Beginner-friendly and extendable
