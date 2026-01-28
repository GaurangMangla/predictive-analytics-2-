# predictive-analytics-2-
Air Quality PDF Estimation using GAN (India Dataset)

This project demonstrates how *Generative Adversarial Networks (GANs)* can be used to estimate the *probability density function (PDF)* of real-world air pollution data.

We use the *India Air Quality Dataset* from Kaggle and apply GAN-based learning to generate synthetic pollutant distributions.

---

## 📌 Project Objective

The goal of this project is:

•⁠  ⁠To collect real NO2 (Nitrogen Dioxide) pollution values  
•⁠  ⁠Normalize the data  
•⁠  ⁠Create noisy observations using user-defined parameters  
•⁠  ⁠Train a GAN model to learn the density distribution  
•⁠  ⁠Compare *Real Data PDF vs GAN Generated PDF*

---

## 📊 Dataset Used

Dataset Name: *India Air Quality Data*  
Source: Kaggle  
Downloaded using: ⁠ kagglehub ⁠

Dataset Link:  
https://www.kaggle.com/datasets/shrutibhargava94/india-air-quality-data

---

## ⚙️ Technologies and Libraries

This project is implemented in *Python* using:

•⁠  ⁠⁠ pandas ⁠ → Data handling  
•⁠  ⁠⁠ numpy ⁠ → Numerical calculations  
•⁠  ⁠⁠ torch ⁠ → GAN model building and training  
•⁠  ⁠⁠ matplotlib ⁠ → Plotting graphs  
•⁠  ⁠⁠ seaborn ⁠ → Density estimation plots  
•⁠  ⁠⁠ kagglehub ⁠ → Direct dataset download  

---

## 🧠 GAN Architecture

### Generator Network
•⁠  ⁠Input: Random noise
•⁠  ⁠Output: Synthetic pollutant values

### Discriminator Network
•⁠  ⁠Input: Real or Fake values
•⁠  ⁠Output: Probability of being real

Both networks compete during training to improve generation quality.

---

## 🔑 UID Based Parameters

The project generates parameters based on the UID:

```python
UID = 102303907

A_VAL = 0.5 * (UID % 7)
B_VAL = 0.3 * (UID % 5 + 1)
