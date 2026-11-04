<div align="center">

# 🇪🇬 Egyptian Currency Recognition

### Deep Learning & Computer Vision for Egyptian Banknote Classification

<p>
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/TensorFlow-Keras-orange?style=for-the-badge&logo=tensorflow&logoColor=white">
  <img src="https://img.shields.io/badge/Computer-Vision-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Deep-Learning-purple?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge">
</p>

**An experimental AI-powered system for recognizing and classifying Egyptian banknotes using traditional Computer Vision techniques and Deep Learning architectures.**

</div>

---

## 📌 Project Overview

Egyptian Currency Recognition is a Computer Vision and Deep Learning project that explores different approaches to identifying Egyptian banknote denominations from images.

The project combines traditional feature extraction techniques with modern deep learning architectures to investigate their effectiveness in currency image classification.

Multiple experiments were implemented using:

- **SIFT (Scale-Invariant Feature Transform)**
- **HOG (Histogram of Oriented Gradients)**
- **Combined SIFT + HOG Feature Extraction**
- **CNN (Convolutional Neural Networks)**
- **EfficientNet Transfer Learning**

The goal is to compare different image representation and classification approaches and evaluate their performance on Egyptian currency images.

## 🎯 Project Objectives

- Build an image classification pipeline for Egyptian banknotes.
- Explore traditional Computer Vision feature extraction techniques.
- Implement CNN-based classification models.
- Apply Transfer Learning using EfficientNet.
- Compare different model architectures and feature extraction strategies.
- Evaluate model performance using classification metrics.
- Investigate image preprocessing and enhancement techniques.

---

## 🚀 Key Features & Technical Approaches

### 1. Image Preprocessing & Enhancement

Image preprocessing techniques are used to improve image quality and prepare the dataset for model training.

The experiments explore:

- Image resizing and normalization.
- Image enhancement and filtering.
- Dataset organization and class balancing.
- Preparing training, validation, and testing datasets.

### 2. SIFT Feature Extraction

SIFT extracts distinctive local features from images.

It helps capture important visual patterns that remain relatively robust under changes in scale and rotation.

### 3. HOG Feature Extraction

Histogram of Oriented Gradients extracts image features based on local gradient orientations.

It represents structural and shape-related information that can help distinguish different banknote categories.

### 4. Combined SIFT + HOG

The project investigates combining SIFT and HOG representations to leverage complementary visual information.

The extracted representations are used in a CNN-based classification experiment.

### 5. EfficientNet Transfer Learning

EfficientNet is explored as a deep learning approach for image classification.

The project includes:

- EfficientNetB0 transfer learning.
- EfficientNetB3 fine-tuning experiments.
- Training and validation monitoring.
- Model evaluation on unseen test images.

---

## 📊 Experimental Results

The following results are reported in the project's notebook experiments.

| Model / Approach | Test Accuracy |
|---|---:|
| SIFT-based CNN | 99.31% |
| HOG-based CNN | 95.52% |
| Combined SIFT + HOG CNN | 99.31% |
| EfficientNetB3 | 86.90% |

**Important:** These are notebook-reported experimental results, not independently reproduced benchmarks. Performance should be interpreted in the context of the dataset size, class distribution, preprocessing pipeline, and train/test split.

The results demonstrate how different feature extraction strategies can influence classification performance.

---

## 💵 Supported Currency Classes

The enhanced classification experiment includes nine categories:

| Class |
|---|
| 1 EGP |
| 5 EGP |
| 10 EGP |
| 10 EGP (New) |
| 20 EGP |
| 20 EGP (New) |
| 50 EGP |
| 100 EGP |
| 200 EGP |

The dataset includes different Egyptian banknote denominations and newer currency variations.

---

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Deep Learning | TensorFlow, Keras |
| Computer Vision | OpenCV |
| Feature Extraction | SIFT, HOG |
| Deep Learning Architectures | CNN, EfficientNet |
| Data Processing | NumPy, Pandas |
| Image Processing | Pillow, Scikit-image |
| Visualization | Matplotlib, Seaborn |
| Evaluation | Scikit-learn |
| Development Environment | Jupyter Notebook |

---

## 📂 Repository Structure

```text
Egyptian_money_detection/
│
├── Egyptian currency/
│
├── Egyptian new currency/
│   └── dataset/
│       ├── train/
│       ├── valid/
│       └── test/
│
├── Euro coins and bills/
│
├── cam.ipynb
├── test.ipynb
│
├── enhanced_money_detection_with_visuals.ipynb
├── improved_money_detection.ipynb
├── filters.ipynb
│
├── combined_sift_hog_model.h5
├── sift_model.h5
├── hog_model.h5
├── efficientnetb0_egyptian_currency_model.h5
│
└── README.md
```

---

## 📓 Notebooks Guide

| Notebook | Description |
|---|---|
| `enhanced_money_detection_with_visuals.ipynb` | Image enhancement, dataset balancing, EfficientNetB3 fine-tuning, and evaluation. |
| `improved_money_detection.ipynb` | EfficientNetB0 transfer learning experiment. |
| `filters.ipynb` | SIFT, HOG, and combined feature extraction experiments. |
| `cam.ipynb` | Model inference and visualization experiments. |
| `test.ipynb` | Testing saved classification models. |

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/nabilamir1/Egyptian_money_detection.git

cd Egyptian_money_detection
```

### 2. Install Dependencies

```bash
pip install tensorflow
pip install opencv-python
pip install numpy pandas
pip install matplotlib seaborn
pip install scikit-learn scikit-image
pip install pillow tqdm
pip install jupyter
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 4. Run the Experiments

Open the desired notebook and execute its cells.

**Note:** Some notebooks contain machine-specific dataset paths. Update the training, validation, and testing directory paths according to your local environment before running them.

Some inference experiments also expect a compatible `label_encoder.pkl` file, which is not included in the repository root.

---

## 🔬 Research & Learning Outcomes

This project provided practical experience in:

- Traditional Computer Vision and feature engineering.
- CNN architecture development.
- Transfer Learning and model fine-tuning.
- Image preprocessing and enhancement.
- Dataset preparation and class balancing.
- Model evaluation and performance comparison.
- Working with TensorFlow/Keras and saved deep learning models.

---

## ⚠️ Current Limitations

- The current implementation focuses on image classification experiments rather than a complete real-time currency detection application.
- Classification performance depends on image quality and dataset representation.
- The reported metrics are specific to the experimental dataset and evaluation setup.
- The models are not designed to verify banknote authenticity or detect counterfeit currency.
- Some notebooks require path configuration and additional inference dependencies.

---

## 🔮 Future Improvements

- Develop a real-time currency recognition application using a webcam or smartphone camera.
- Explore YOLO-based banknote detection.
- Improve model generalization with larger and more diverse datasets.
- Optimize trained models for mobile and edge-device deployment.
- Integrate Text-to-Speech for accessible currency recognition.
- Build a user-friendly interface for practical testing.

---

## 👨‍💻 Developer

**Nabil Amir**

Artificial Intelligence & Computer Science Student  
AI | Machine Learning | Deep Learning | Computer Vision

**GitHub:** nabilamir1

**Portfolio:** nabilamir1.github.io/portfolio/

---

<div align="center">

### Built with Python, Computer Vision & Deep Learning 🇪🇬

**Exploring AI-powered solutions for Egyptian currency recognition.**

</div>
