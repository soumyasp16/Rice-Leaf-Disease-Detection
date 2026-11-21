# 🌾 Rice Leaf Disease Detection

## 📌 Project Overview

Rice Leaf Disease Detection is a Machine Learning and Deep Learning project developed to classify rice leaf diseases using digital images.

The main objective of this project is to identify three major rice leaf diseases using image processing, Machine Learning algorithms, Convolutional Neural Networks (CNN), Data Augmentation, and Transfer Learning.

This project explores different classification models, compares their performance, and identifies the most suitable model for rice leaf disease classification.

## 🎯 Problem Statement

To develop an image classification model that can identify the following three rice leaf diseases:

1. Leaf Smut
2. Brown Spot
3. Bacterial Leaf Blight

**Note:** The original problem statement mentions Leaf Blast, but the provided dataset contains Leaf Smut instead. Therefore, this project uses the three actual dataset categories.

## 📂 Dataset Information

The dataset contains 119 images of disease-infected rice leaves, divided equally into three categories.

| Disease Category | Number of Images |
|---|---:|
| Leaf Smut | 40 |
| Brown Spot | 40 |
| Bacterial Leaf Blight | 39 |
| **Total** | **119** |

**Dataset Source:**

[Download Rice Leaf Disease Dataset](https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1001-RiceLeaf.zip)

## 🛠️ Technologies and Libraries Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- OpenCV
- Pillow
- Scikit-learn
- TensorFlow
- Keras
- Joblib

## 🔍 Project Workflow

### 1. Data Collection
Collected rice leaf disease images from the provided dataset.

### 2. Exploratory Data Analysis (EDA)
- Analyzed the dataset structure.
- Checked disease class distribution.
- Visualized sample images.
- Analyzed image dimensions and formats.
- Checked missing and corrupted images.

### 3. Image Preprocessing
- Resized images to 224 × 224 pixels.
- Converted images into RGB format.
- Normalized pixel values.
- Divided the dataset into training, validation, and testing sets.

### 4. Feature Extraction
Used Histogram of Oriented Gradients (HOG) to extract image features for traditional Machine Learning algorithms.

### 5. Model Building

Implemented the following classification models:

- HOG + Support Vector Machine (SVM)
- Random Forest Classifier
- Convolutional Neural Network (CNN)
- CNN with Data Augmentation
- MobileNetV2 using Transfer Learning

### 6. Data Augmentation

Applied different image augmentation techniques:

- Horizontal Flipping
- Random Rotation
- Random Zoom
- Random Translation
- Random Contrast

### 7. Model Evaluation

Evaluated model performance using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 8. Model Comparison

Compared the performance of all implemented models to identify the best-performing candidate.

## 📊 Model Performance Comparison

Five different Machine Learning and Deep Learning models were implemented and evaluated using Accuracy, Precision, Recall, and F1-score.

### Performance Results

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| HOG + SVM | 66.67% | 66.67% | 66.67% | 65.71% |
| Random Forest | 55.56% | 53.70% | 55.56% | 52.96% |
| CNN | 72.22% | 78.52% | 72.22% | 73.13% |
| CNN + Augmentation | 55.56% | 55.56% | 55.56% | 54.60% |
| **MobileNetV2** | **88.89%** | **91.67%** | **88.89%** | **88.57%** |

### 🏆 Best Performing Model: MobileNetV2

Based on the experimental results, MobileNetV2 achieved the best overall performance among the five evaluated models.

- **Accuracy:** 88.89%
- **Precision:** 91.67%
- **Recall:** 88.89%
- **F1-Score:** 88.57%

### Model Comparison Analysis

1. **HOG + SVM:** Achieved 66.67% accuracy using traditional image feature extraction.
2. **Random Forest:** Achieved 55.56% accuracy, showing comparatively lower classification performance.
3. **CNN:** Achieved 72.22% accuracy by learning image features automatically.
4. **CNN + Augmentation:** Achieved 55.56% accuracy in this experiment. Augmentation did not improve performance, possibly because of the very small dataset and training configuration.
5. **MobileNetV2:** Achieved the highest accuracy of 88.89% and the highest precision of 91.67%.

### Final Model Selection

MobileNetV2 was selected as the best-performing candidate based on its accuracy, precision, recall, and F1-score.

Transfer learning helped leverage pretrained image features, making it a promising approach for this small rice leaf disease dataset.

**Note:** These results are based on a test set of only 18 images. Therefore, further validation using a larger and independent dataset is recommended before real-world production deployment.
## 📈 Project Results

The project generates the following visualizations:

- Disease Class Distribution
- Sample Rice Leaf Images
- Image Dimension Analysis
- CNN Training Accuracy and Loss
- Data Augmentation Examples
- Model Performance Comparison
- Confusion Matrices

## 📁 Project Structure

```text
Rice-Leaf-Disease-Detection/
│
├── notebooks/
│   └── RiceLeaf_Disease_Detection.ipynb
│
├── models/
│   └── Saved trained models
│
├── results/
│   ├── class_distribution.png
│   ├── model_comparison.png
│   └── confusion_matrix.png
│
├── Dataset/
│   └── Disease image folders
│
├── README.md
├── requirements.txt
└── .gitignore
```

## ⚙️ Installation and Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Rice-Leaf-Disease-Detection.git
```

### Step 2: Navigate to the Project Folder

```bash
cd Rice-Leaf-Disease-Detection
```

### Step 3: Install Required Libraries

```bash
pip install -r requirements.txt
```

### Step 4: Download the Dataset

Download the dataset using the link provided above and extract the images into the Dataset folder.

### Step 5: Open Jupyter Notebook

```bash
jupyter notebook
```

Open the following notebook:

`notebooks/RiceLeaf_Disease_Detection.ipynb`

Run the notebook cells sequentially.

## 🚧 Challenges Faced and Solutions

| Challenges | Solutions |
|---|---|
| Limited dataset containing 120 images | Applied Data Augmentation |
| Different image dimensions | Resized images to 224 × 224 |
| Pixel value variations | Applied normalization |
| Overfitting risk | Used Dropout and Data Augmentation |
| Similar disease patterns | Experimented with CNN and Transfer Learning |
| Model selection | Compared multiple evaluation metrics |

## 🏁 Conclusion

The Rice Leaf Disease Detection project demonstrates the use of Machine Learning and Deep Learning techniques for classifying rice leaf diseases.

Different classification algorithms were implemented and evaluated using various performance metrics.

Data Augmentation and Transfer Learning were explored to improve model generalization.

The final model was selected based on experimental performance.

This project provides practical experience in image preprocessing, Exploratory Data Analysis, feature extraction, model building, and performance evaluation.

## 🔮 Future Improvements

- Increase the number of rice leaf images.
- Include more rice disease categories.
- Improve model generalization using larger datasets.
- Develop a web-based disease prediction application.
- Develop an Android application.
- Deploy the selected model for real-world testing.

---

⭐ If you find this project useful, please consider giving the repository a star!