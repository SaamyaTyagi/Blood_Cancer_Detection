# Early-Stage Blood Cancer Detection Using Microscopic Cell Images

This project explores the use of classical and deep learning techniques to detect early-stage leukemia from high-resolution microscopic blood cell images.

---

## About the Dataset

The dataset consists of high-resolution (1024x1024+) Wright-Giemsa stained blood smear images captured at 100x oil immersion magnification. It includes:

- **Myeloblasts** (AML indicators): 12-20 micrometers in size, round to oval shape, high nuclear-cytoplasm ratio, with visible nucleoli  
- **Lymphoblasts** (ALL indicators): 10-14 micrometers, homogeneous chromatin, minimal cytoplasm  
- **Normal Cells**: Includes mature lymphocytes, neutrophils, monocytes, eosinophils, and basophils  
- Images are 24-bit RGB and include multiple focal planes per sample

---

## Project Objective

Develop a robust machine learning pipeline for early-stage blood cancer detection by integrating both handcrafted and deep learning-based feature extraction techniques for improved classification accuracy.

---

## Approach

### Feature Extraction
- **Handcrafted Features**: Extracted detailed texture features using Local Binary Patterns (LBP) and Gray-Level Co-occurrence Matrix (GLCM)
- **Deep Semantic Features**: Extracted using a pre-trained ResNet18 model

### Modeling
- Trained Support Vector Machine (SVM) and Multi-Layer Perceptron (MLP) classifiers on the combined feature sets
- Evaluated performance using standard metrics such as accuracy, precision, recall, and F1-score

---

## Results

- Improved validation accuracy from 96% (SVM) to 98.1% (MLP), representing a 2.1% performance gain across over 1,000 test samples
- Achieved 97% precision and recall across all five blood cell types, demonstrating the effectiveness of the hybrid feature fusion approach

---

## Tech Stack

- **Languages/Tools**: Python, OpenCV, NumPy, Scikit-learn  
- **Deep Learning Framework**: PyTorch (using ResNet18)  
- **Visualization**: Matplotlib, Seaborn

---

## Made By:

Saamya Tyagi, under guidance of Prof. Anshuman Tyagi 
