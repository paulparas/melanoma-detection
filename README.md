# Melanoma Detection using Convolutional Neural Networks

## Problem Statement
This project aims to build a custom convolutional neural network (CNN) model using TensorFlow to detect melanoma, a type of skin cancer that is highly dangerous and can be fatal if not diagnosed early. Melanoma accounts for 75% of skin cancer deaths, highlighting the need for advanced diagnostic solutions. This CNN model seeks to automate the detection process, potentially alerting dermatologists to the presence of melanoma and significantly reducing the manual effort required for diagnosis.

## Dataset
The dataset used in this project can be downloaded from [here](#). It includes 2357 images of malignant and benign skin conditions sourced from the International Skin Imaging Collaboration (ISIC). The images are classified according to ISIC standards, with melanomas and moles being slightly more predominant in the dataset.

### Conditions covered in the dataset:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Project Pipeline
1. **Data Reading/Data Understanding**:
   - Define paths for training and testing images.

2. **Dataset Creation**:
   - Create training and validation datasets with a batch size of 32 and resize images to 180x180 pixels.

3. **Dataset Visualization**:
   - Implement code to visualize one instance from each of the nine classes.

4. **Model Building & Training**:
   - Build a CNN to detect the nine classes, normalizing pixel values between 0 and 1.
   - Select an appropriate optimizer and loss function.
   - Train the model for approximately 20 epochs.
   - Analyze the model for any signs of overfitting or underfitting.

5. **Data Augmentation**:
   - Apply data augmentation strategies to address any issues of model fitting.

6. **Handling Class Imbalances**:
   - Use the Augmentor library to balance the class distribution in the training data.

7. **Model Building & Training on Augmented Data**:
   - Rebuild and retrain the CNN on the augmented dataset for about 30 epochs.
   - Evaluate the effectiveness of the modifications.

8. **Class Distribution Analysis**:
   - Examine and address any imbalance in class distribution within the training dataset.

## Note
- The model should be built from scratch, without using pre-trained models or transfer learning.
- The use of GPU runtime in Google Colab is advised due to the extensive training periods required.

## Conclusion
This project is designed as an educational tool to understand the mechanics of CNNs and their application in a real-world problem of melanoma detection. Users are encouraged to explore the base code, adapt it to their needs, and improve upon the model's accuracy and efficiency.
