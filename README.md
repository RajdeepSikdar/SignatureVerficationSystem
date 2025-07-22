# 🖊️ Handwritten Signature Verification Using Deep Learning

## 📄 Overview
This project presents a deep learning-based approach for verifying handwritten signatures using Convolutional Neural Networks (CNNs) and Siamese architecture. It aims to enhance accuracy, reduce false acceptances/rejections, and provide a scalable biometric solution for real-world applications.

## 👥 Authors
- **Deesha Mitra** – UG Student, CSE, Presidency University  
- **Rajdeep Sikdar** – UG Student, CSE, Presidency University  

## 🧠 Methodology
### 🔹 Dataset Preparation
- Two folders: `Original` and `Forged` signatures
- Images resized to **150x150**, converted to **grayscale**, and normalized
- Dataset split into:
  - Training pairs: 290  
  - Validation pairs: 34  
  - Test pairs: 82  

### 🔹 Pair Generation
- Positive and negative pairs created for Siamese network training

### 🔹 Model Architecture
- Siamese network with twin CNNs
- Feature vectors compared using a distance metric
- Final layer outputs similarity score

### 🔹 Training
- Loss function: Binary Crossentropy  
- Optimizer: Adam  
- Epochs: 50  
- Achieved Accuracy: **92.4%**

## 📊 Results

| Metric     | Value   |
|------------|---------|
| Accuracy   | 92.4%   |
| Precision  | 91.8%   |
| Recall     | 93.1%   |
| F1-Score   | 92.4%   |

- Model shows strong convergence and minimal overfitting
- Threshold similarity score: **0.5**
  - Score ≥ 0.5 → Genuine Signature  
  - Score < 0.5 → Forged Signature  

## 🛠️ Technologies Used
- Python  
- TensorFlow / Keras  
- OpenCV  
- Google Colab  

## 🌍 Real-World Applications
- **Banking**: Check & transaction verification  
- **Legal**: Contract & affidavit authentication  
- **Corporate**: HR & expense approvals  
- **Healthcare**: Prescription & insurance verification  
- **Education**: Exam & certificate validation  

## 🚀 Future Enhancements
- Multi-modal authentication (pressure, stroke dynamics)
- Mobile SDKs for real-time verification
- Blockchain integration for secure storage
- Cloud-based APIs for scalable deployment

## 📦 Business Potential
- SaaS for banks and legal firms  
- Government tenders for ID/passport verification  
- HIPAA-compliant healthcare solutions  
- Integration with DocuSign and IoT devices  

## 📚 References
- Hafemann et al. (2017), Diaz et al. (2021), Bromley et al. (1993), and others  
- Dataset sourced from [Kaggle](https://www.kaggle.com)

## 📁 Repository Structure (Suggested)
