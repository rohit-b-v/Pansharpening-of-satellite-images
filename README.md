# 🛰️ Pansharpening of Satellite Images  
**Automatic Land Cover Change Detection and Analysis System from High-Resolution Remote Sensing Images**

---

## 📌 Overview  
This project develops an **automatic land cover change detection and analysis system** using **high-resolution satellite images**, with a focus on **pansharpening** — a technique that enhances spatial resolution of multispectral imagery by fusing it with high-resolution panchromatic images.  

Traditional pansharpening methods (e.g., Brovey, ESRI transformations) often fail to generalize across datasets. Modern deep learning approaches, such as CNNs and autoencoders, improve performance but still face challenges in robust feature extraction and reconstruction. This project implements a **deep learning-based pansharpening model** that combines the strengths of both multispectral and panchromatic imagery for accurate land cover analysis.  

---

## 🛠️ Tech Stack  
- **Languages:** Python  
- **Libraries/Frameworks:** TensorFlow / Keras, NumPy, OpenCV  
- **Techniques:** CNNs, Autoencoders, Image Fusion, Gaussian Blurring, Downsampling  

---

## 📂 Dataset & Preprocessing  
- **Inputs:**  
  - Multispectral images: `512 × 512 × 3`  
  - Panchromatic images: `512 × 512`  
- **Preprocessing steps:**  
  - Calculation of scaling factors  
  - Gaussian blurring for interpolation  
  - Spatial downsampling  
  - Splitting into smaller patches (`64 × 64`) for efficient training  

---

## ⚙️ Model Architecture  
The model consists of **three key blocks**:  
1. **Multispectral Block** – extracts features from multispectral inputs  
2. **Panchromatic Block** – captures spatial features from high-resolution panchromatic inputs  
3. **Fusion Block** – combines outputs to generate pansharpened high-resolution images  

- Layers: Convolution + Pooling  
- Activation: **Swish**  
- Loss Function: **Mean Squared Error (MSE)**  
- Optimizer: **Adam**  

---

## Screenshots

<img width="540" height="179" alt="image" src="https://github.com/user-attachments/assets/95d91168-c7c8-4b16-afe9-3699cb7b739f" />

