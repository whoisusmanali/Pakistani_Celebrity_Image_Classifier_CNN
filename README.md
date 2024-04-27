# Pakistani Celebrity Image Classifier CNN

This project involves building a Convolutional Neural Network (CNN) to classify images of Pakistani celebrities. The dataset was collected using the Chrome Extension "Download All Images" and underwent several preprocessing steps before model training.

## Libraries/Dependencies:
1. OpenCV (`cv2`)
2. NumPy
3. Matplotlib
4. os
5. shutil
6. TensorFlow
7. Keras
8. imghdr

# Project Workflow:

## 1. Importing Libraries:
All necessary libraries are imported at the beginning of the script for clarity and reproducibility.

## 2. Data Cleaning:
Data cleaning is essential for preparing the dataset for training. This step involves:
- Utilizing pre-trained Haar Cascade XML files to detect and crop faces in images.
- Deleting images where the cropped face does not belong to the intended celebrity.
- Removing blurry or low-quality images that may hinder model performance.

## 3. Image Preprocessing:
A preprocessing function is applied to handle images with incorrect formats and ensure uniformity in the dataset.

## 4. Data Pipeline:
The dataset is processed into batches using TensorFlow's Keras utilities to streamline model training.

## 5. Image Scaling:
Images are scaled to a consistent size to facilitate model training, as CNNs typically require inputs of uniform dimensions.

## 6. Data Splitting:
The dataset is divided into training, testing, and validation sets with proportions of 70%, 20%, and 10%, respectively.

## 7. Model Building:
The CNN architecture consists of:
- Six convolutional (`Conv2D`) layers followed by max-pooling layers for feature extraction.
- A flattening layer to transform the data into a 1D array.
- Two dense (`Dense`) layers for classification, with the output layer using the softmax activation function for multi-class classification.
The model is compiled with sparse categorical cross-entropy loss and the Adam optimizer.

## 8. Performance Evaluation:
The model demonstrates high accuracy, achieving 98.44% accuracy with minimal loss (0.06).

# Screenshots:

![Screenshot of Data Cleaning](https://user-images.githubusercontent.com/104086680/232634486-ff0c5208-4577-4fd5-88f2-0d16147bfe20.png)

### Model Architecture:

![Screenshot of Model Architecture](https://user-images.githubusercontent.com/104086680/232634611-4b5eb858-6627-4cdc-a5d8-49f455c912fd.png)

---

## Importing the Repository to Local Environment and Usage:

### 1. Clone the Repository:
```bash
git clone https://github.com/your-username/your-repository.git
```

### 2. Navigate to the Repository:
```bash
cd your-repository
```
### 3. Install Dependencies:
```bash
pip install -r requirements.txt
```
## 4. Run the Script:
```bash
python main.py
