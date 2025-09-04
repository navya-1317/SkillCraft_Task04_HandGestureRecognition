# SkillCraft Task 04 – Hand Gesture Recognition

## 🎯 Objective
Develop a hand gesture recognition model that can accurately identify and classify different hand gestures from image or video data, enabling intuitive human–computer interaction and gesture-based control systems.

---

## 📂 Dataset
- **Dataset Name:** LeapGestRecog (Kaggle)
- Contains grayscale gesture images across multiple gesture classes.

---

## 🛠 Steps Taken
1. **Dataset Loading**
   - Downloaded dataset from Kaggle using `kagglehub`.
   - Extracted and organized into structured directory format.

2. **Data Preprocessing**
   - Resized images to a fixed dimension `(128x128)`.
   - Converted to grayscale to reduce complexity.
   - Normalized pixel values.
   - Split into Train, Validation, and Test sets.

3. **Data Augmentation**
   - Applied random flips, rotations, and zoom to improve generalization.

4. **Model Building**
   - Constructed a Convolutional Neural Network (CNN) with:
     - Multiple Conv2D + MaxPooling layers
     - Dropout layers to prevent overfitting
     - Fully connected Dense layers
   - Output layer with softmax activation for multi-class classification.

5. **Training**
   - Used Adam optimizer, categorical cross-entropy loss.
   - Early stopping and model checkpointing applied.

6. **Evaluation**
   - Measured accuracy on validation and test datasets.
   - Visualized confusion matrix.
   - Tested on a sample image.

---

## 📊 Final Results
- **Train Epochs:** 7
- **Best Validation Accuracy:** 43.75%
- **Test Accuracy:** 43.75%
- **Sample Prediction:** Predicted class matched actual class in example.

---



## 📌 Insights
- Model performed modestly, indicating potential improvement with:
  - More training epochs
  - Transfer learning from pre-trained CNNs
  - More data augmentation
- Successfully built an end-to-end pipeline for gesture recognition.

---

