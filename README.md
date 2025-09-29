# Pneumonia Detection from Chest X-Rays 🩺💻

## Project Overview
This project uses **deep learning** to detect pneumonia from chest X-ray images. We leverage **transfer learning** with **MobileNetV2** to achieve high accuracy while using limited computational resources.

## Dataset
- Chest X-ray images labeled as **Normal** or **Pneumonia**.
- Data preprocessing includes:
  - **Resizing** images
  - **Normalization**
  - **Augmentation** (rotation, flipping, etc.) to improve generalization

## Model
- Base: **MobileNetV2** (pretrained on ImageNet)
- Added layers:
  - Global Average Pooling
  - Dense layer (128 units, ReLU)
  - Dropout (0.5)
  - Output layer (sigmoid for binary classification)
- Optimizer: Adam
- Loss: Binary Crossentropy

## Training & Evaluation
- Training was done on **Google Colab (free GPU)**.
- Test accuracy: **89% ✅**
- Additional evaluation metrics:
  - Precision
  - Recall
  - F1-score
  - Confusion matrix
- Observed some misclassifications, but overall model performance is strong.

## Future Work
- Experiment with different architectures (e.g., ResNet, EfficientNet)
- Fine-tune more layers
- Increase dataset size to improve accuracy and robustness

## Conclusion
This project demonstrates that **deep learning can assist medical diagnosis** effectively, even with limited resources. 🚑


