#  Airborne Object Detection with GAN Augmentation

##  Project Overview

This project focuses on classifying airborne objects using a Convolutional Neural Network (CNN).

The dataset includes four classes:

-  Airplane  
-  Bird  
-  Drone  
-  Helicopter  

To improve classification performance, especially for difficult classes, **Generative Adversarial Networks (GANs)** were used for data augmentation.

---

##  Objective

The main goal is to:

> Improve classification performance using GAN-based synthetic data augmentation

---

##  Methodology

### 1️ Baseline Model
- A CNN model was trained using the original dataset
- Evaluation was done using:
  - Test accuracy
  - Confusion matrix

---

### 2️ GAN Training
- A DCGAN model was trained on helicopter images  
- The generator learned to produce realistic helicopter samples  

---

### 3️ Data Augmentation
- Generated synthetic helicopter images  
- Combined them with the original dataset:
    
---

### 4️ Retraining CNN
- CNN model retrained using augmented dataset  
- Same architecture and settings used for fair comparison  

---

## Results

###  Baseline vs GAN-Augmented

| Metric | Baseline | GAN-Augmented |
|--------|----------|---------------|
| Helicopter Accuracy | Lower | Higher  |
| Misclassification (→ Airplane) | High | Reduced |

---

###  Key Improvement

> Misclassification of helicopters as airplanes significantly decreased  

GAN helped the model learn more distinctive helicopter features.

---

##  Technologies Used

- Python  
- PyTorch  
- Torchvision  
- Google Colab  
- Matplotlib  
- Scikit-learn  

---


---

## Conclusion

GAN-based data augmentation proved effective in improving the classification of helicopters.

The model showed better generalization and reduced confusion with similar classes.

