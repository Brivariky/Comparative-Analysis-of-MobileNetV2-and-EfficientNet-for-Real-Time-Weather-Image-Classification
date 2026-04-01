🌦️ Comparative Analysis of MobileNetV2 and EfficientNet for Real-Time Weather Image Classification
📌 Overview

This project focuses on comparing two efficient deep learning models, MobileNetV2 and EfficientNetB0, for real-time weather image classification. The goal is to evaluate their performance in terms of both accuracy and computational efficiency, making them suitable for deployment in real-world applications such as mobile or edge devices.

🧠 Models Used
MobileNetV2
Lightweight architecture using inverted residual blocks
Optimized for fast inference and low resource usage
EfficientNetB0
Uses compound scaling (depth, width, resolution)
Designed for a balance between accuracy and efficiency
⚙️ Methodology
Transfer learning using ImageNet-pretrained models
Fine-tuning the top layers while keeping lower layers frozen
Identical classification head for fair comparison
Input images resized to 224 × 224
Data augmentation applied to improve generalization
📊 Evaluation Metrics

Models are evaluated using:

Accuracy
Precision
Recall
F1-Score
Inference Time (for real-time performance)
🎯 Objective

To analyze the trade-off between speed and accuracy and determine which model is more suitable for real-time weather classification tasks.

🚀 Key Insight
MobileNetV2 → Faster, lightweight, ideal for mobile deployment
EfficientNetB0 → More balanced, potentially higher accuracy
