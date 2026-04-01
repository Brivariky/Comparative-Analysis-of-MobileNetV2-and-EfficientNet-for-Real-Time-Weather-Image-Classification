# 🌦️ Comparative Analysis of MobileNetV2 and EfficientNet for Real-Time Weather Image Classification

## 📌 Overview
This project presents a comparative study of two efficient deep learning models, **MobileNetV2** and **EfficientNetB0**, for real-time weather image classification. The objective is to evaluate their performance in terms of **accuracy** and **computational efficiency**, making them suitable for deployment in real-world applications such as mobile and edge devices.

## 🧠 Models
### MobileNetV2
- Lightweight architecture with inverted residual blocks  
- Optimized for low latency and mobile environments  

### EfficientNetB0
- Compound scaling of depth, width, and resolution  
- Balanced trade-off between accuracy and efficiency  

## ⚙️ Methodology
- Transfer learning using ImageNet-pretrained models  
- Fine-tuning upper layers while freezing lower layers  
- Identical classification head for fair comparison:
  - Global Average Pooling  
  - Dropout (0.5 → 0.3)  
  - Fully Connected Layers  
  - Softmax output (4 classes)  
- Input size: 224 × 224  
- Data augmentation:
  - Horizontal flip  
  - Brightness adjustment  

## 📂 Dataset
- Source: Kaggle Weather Dataset  
- Classes:
  - Sunny  
  - Cloudy  
  - Foggy  
  - Rainy  
- Split:
  - Train: 70%  
  - Validation: 15%  
  - Test: 15%  

## 📊 Evaluation Metrics
- Accuracy – overall correctness  
- Precision – reliability of predictions  
- Recall – ability to capture relevant samples  
- F1-Score – balance between precision and recall  
- Inference Time – processing speed per image  

## 🏋️ Training Configuration
- Framework: PyTorch (CUDA)  
- Optimizer: Adam  
- Learning rate: 1e-4  
- Weight decay: 1e-4  
- Batch size: 32  
- Epochs: 30 (with early stopping)  

## 📈 Workflow
1. Dataset preparation  
2. Preprocessing (resize + normalization)  
3. Data augmentation  
4. Model training (transfer learning + fine-tuning)  
5. Model evaluation  
6. Model comparison  

## 🎯 Objective
To analyze the trade-off between **accuracy** and **inference speed** and determine the most suitable model for real-time weather classification.

## 📎 License
For academic and research purposes only.
