# 🩺 Decision Fusion for Ear-Drum Abnormality Detection Using Otoscopic Images and Tympanometry

A multimodal machine learning system that combines **deep learning** and **traditional machine learning** to improve the diagnosis of ear-drum abnormalities. The project leverages **VGG19** for otoscopic image analysis and **Random Forest** for tympanometry data classification, followed by a **decision fusion** strategy to enhance diagnostic performance.

---

## 📌 Project Overview

Accurate diagnosis of ear-drum abnormalities is essential for timely treatment and prevention of hearing-related complications. Conventional diagnosis relies on otoscopic examination and tympanometry independently, each providing different but complementary clinical information.

This project integrates both modalities using a **Decision Fusion** approach, enabling more reliable predictions than using a single diagnostic method.

---

## 🎯 Objectives

- Detect ear-drum abnormalities from otoscopic images.
- Analyze tympanometry measurements using machine learning.
- Combine predictions from both models using Decision Fusion.
- Improve diagnostic accuracy through multimodal learning.

---

## 🏗️ System Architecture

```
                Otoscopic Images
                       │
                       ▼
                Image Preprocessing
                       │
                       ▼
                  VGG19 CNN Model
                       │
                Prediction Scores
                       │
                       ▼
                Decision Fusion
                       ▲
                       │
              Random Forest Model
                       ▲
                       │
           Tympanometry Peak Values
```

---

## 🧠 Models Used

### 🔹 VGG19 (Deep Learning)

- Transfer Learning using pretrained VGG19
- Feature extraction from otoscopic images
- Image preprocessing and normalization
- Classification of ear-drum conditions

### 🔹 Random Forest

- Trained on tympanometry peak-value dataset
- Ensemble learning using multiple decision trees
- Classifies middle-ear conditions from clinical measurements

### 🔹 Decision Fusion

The outputs from both models are combined using a fusion strategy to generate the final diagnosis.

Fusion techniques include:

- Average Probability Fusion
- Weighted Score Fusion

This multimodal approach improves robustness and diagnostic reliability.

---

## 📂 Dataset

The project uses two different datasets:

### 📷 Otoscopic Image Dataset

- Training Images
- Validation Images
- Testing Images

### 📈 Tympanometry Dataset

Contains peak-value measurements extracted from tympanograms for machine learning classification.

---

## ⚙️ Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📊 Workflow

1. Load otoscopic image dataset
2. Preprocess images
3. Train VGG19 model
4. Load tympanometry dataset
5. Train Random Forest classifier
6. Evaluate both models independently
7. Perform Decision Fusion
8. Generate final prediction
9. Evaluate overall system performance

---

## 📈 Results

The project evaluates performance using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

The decision fusion framework demonstrates improved diagnostic reliability by integrating visual and clinical information.

---

## 📁 Project Structure

```
Decision-Fusion-Ear-Diagnosis/
│
├── Decision_Fusion_Ear_Diagnosis.ipynb
├── README.md
├── requirements.txt
├── .gitignore
├── dataset/
│   ├── train/
│   ├── validation/
│   ├── test/
│   └── dataset2.csv
├── saved_model/
│   └── modelVGG19.keras
└── images/
    ├── accuracy.png
    ├── loss.png
    ├── confusion_matrix.png
    └── architecture.png
```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Decision-Fusion-Ear-Diagnosis.git
```

Move into the project directory:

```bash
cd Decision-Fusion-Ear-Diagnosis
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
Decision_Fusion_Ear_Diagnosis.ipynb
```

---

## 💡 Applications

- AI-assisted clinical diagnosis
- Smart healthcare systems
- Telemedicine platforms
- ENT decision support systems
- Medical image analysis
- Computer-aided diagnosis

---

## 🔮 Future Enhancements

- Integrate larger and more diverse datasets.
- Deploy the model as a web application using Flask or Streamlit.
- Develop a mobile-based diagnostic assistant.
- Improve explainability using Grad-CAM and Explainable AI (XAI).
- Extend the framework to classify additional ear diseases.

---

## 👨‍💻 Authors

**P. Thanusha Reddy**

B.Tech Electronics and Communication Engineering

Amrita Vishwa Vidyapeetham

---

## 📄 License

This project is intended for educational and research purposes.
