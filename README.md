# 🌼 Flower Image Classifier

A deep learning model that classifies images of flowers into five categories using **transfer learning** (MobileNetV2) and the `tf_flowers` dataset.

---

## 🔍 Project Overview

- ✅ Pretrained MobileNetV2 (transfer learning)  
- ✅ TensorFlow Datasets integration  
- ✅ Image resizing, batching, and normalization  
- ✅ Accuracy visualization and confusion matrix  
- ✅ Image upload and prediction demo in Colab  

---

## 🌸 Dataset

- **Source**: [`tf_flowers`](https://www.tensorflow.org/datasets/catalog/tf_flowers) via TensorFlow Datasets  
- **Classes**: `daisy`, `dandelion`, `roses`, `sunflowers`, `tulips`  
- **Size**: ~3,600 labeled images  

---

## 🧠 Model Architecture

- Base: `MobileNetV2` (pretrained on ImageNet)
- Layers:
  - GlobalAveragePooling2D  
  - Dense(128, ReLU)  
  - Dense(5, Softmax)
- Loss: Sparse Categorical Crossentropy  
- Optimizer: Adam

---

## 📊 Evaluation

- Validation accuracy: **~90%**  
- Confusion matrix for detailed class performance  
- Prediction confidence displayed for uploaded images

---

## 🖼️ Try It in Colab

1. Open `05_predict_custom_image.ipynb`
2. Upload your image (JPG/PNG)
3. Model will display predicted flower type and confidence

```python
🌻 Predicted: Sunflower
Confidence: 96.2%
