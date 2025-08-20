# Feature‑Rich Deep Learning Architecture for Breast Cancer Detection

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mswastika/Feature-Rich-Deep-Learning-Architecture-for-Breast-Cancer-Detection-/blob/main/notebooks/Another_copy_of_MAJOR_PROJECT_BREAST_CANCER_ANALYSIS_F.ipynb)

A Colab-friendly project for **breast cancer classification** on ultrasound images. It compares **hand‑crafted features** (GLCM, LBP, Intensity) with **deep models** (VGG16, ResNet18, ResNet50) and evaluates using **classification report, confusion matrix, and ROC curves**.

---

## 📦 Folder Structure
```
.
├── notebooks/
│   └── Another_copy_of_MAJOR_PROJECT_BREAST_CANCER_ANALYSIS_F.ipynb
├── images/                # (optional) saved plots
├── requirements.txt
├── README.md
└── LICENSE
```

## 🚀 Quick Start (Colab)
1. Click the **Open in Colab** badge above.
2. Upload your dataset to **Google Drive**.
3. Mount Drive in the first cell:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   DATA_DIR = '/content/drive/MyDrive/<path-to-your-dataset>'
   ```
4. Run cells in order:
   - Preprocessing (resize → grayscale → label encoding)
   - Feature Extraction (GLCM, LBP, Intensity)
   - Model Training (VGG16/ResNet18/ResNet50)
   - Evaluation (classification report, confusion matrix, ROC)

## 🧰 Local Setup (Optional)
```bash
git clone https://github.com/mswastika/Feature-Rich-Deep-Learning-Architecture-for-Breast-Cancer-Detection-.git
cd Feature-Rich-Deep-Learning-Architecture-for-Breast-Cancer-Detection-
pip install -r requirements.txt
```

## 📊 Save & Upload Your Results
In Colab, save plots like this and then upload `images/` to GitHub.
```python
import matplotlib.pyplot as plt
# ... your plotting code ...
plt.savefig('confusion_matrix.png', dpi=150, bbox_inches='tight')
```
Create an `images/` folder in your repo and add the saved PNGs.

## 📝 Dataset
- 3 classes: **Benign**, **Malignant**, **Normal**
- Remove duplicates/masked images, resize to consistent size, grayscale if required.
- Make sure your code points to the dataset folder in Drive (`DATA_DIR`).

## ✅ Requirements
Install from `requirements.txt` or copy the list below:
```
numpy
pandas
matplotlib
seaborn
scikit-learn
opencv-python
tensorflow
keras
```

## 🧪 Results to Report
- Accuracy, Precision, Recall, F1‑score
- Confusion Matrix (per model/feature set)
- ROC‑AUC per class

## 👩‍💻 Authors
- Somali Saha
- Swastika Mondal
- Rakhi Saha
- Jagannath Mondal
- Sudip Chatterjee

## ⚖️ License
Released under the **MIT License** (see `LICENSE`).

---

> Tip: If your repo path or notebook name changes, update the Colab badge link at the top.
