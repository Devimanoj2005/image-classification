# Simple Image Classification with OpenCV & SVM

## Objective
The goal of this project is to build a **simple image classification system** using OpenCV for image preprocessing and a machine learning model (Support Vector Machine) for classification.  
This project also demonstrates basic image manipulation techniques like brightness and contrast adjustment, grayscale conversion, and filtering.

---

## Dataset
- **Dataset used:** CIFAR-10
- **Description:** CIFAR-10 is a widely-used dataset consisting of **60,000 32x32 color images** in **10 classes** (airplane, car, bird, cat, deer, dog, frog, horse, ship, truck).  
- **Train/Test split:** 50,000 training images, 10,000 testing images

---

## Preprocessing Steps
1. **Load the dataset** using `tensorflow.keras.datasets.cifar10`.
2. **Convert images to grayscale** to reduce complexity.
3. **Normalize pixel values** to the range `[0, 1]`.
4. **Enhance images** using brightness and contrast adjustment with OpenCV (`cv2.convertScaleAbs`).
5. **Flatten images** for input into machine learning models like SVM.

---

## Model Used
- **Algorithm:** Support Vector Machine (SVM)  
- **Kernel:** Linear  
- **Training:** Subset of 5,000 images from training set (to reduce runtime)  
- **Evaluation:** 1,000 images from the test set

---

## Model Evaluation
- **Accuracy:** The model predicts test images with an accuracy printed in the notebook.  
- **Confusion Matrix:** Shows the correct and incorrect predictions across all 10 classes.  

---

## Visualization
- **Preprocessing Visualization:**  
  - Original images  
  - Grayscale conversion  
  - Brightness/contrast enhanced images  
- **Prediction Visualization:**  
  - Test images shown with predicted vs actual labels  
- **Example Output:** (Screenshots can be added here if needed)

---

## How to Run
1. Clone the repository:

```bash
git clone https://github.com/Devimanoj2005/image-classification.git
cd image-classification
