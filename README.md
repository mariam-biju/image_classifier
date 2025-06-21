# 🌼 Flower Image Classifier

A deep learning project that classifies flower images into one of five categories:

Daisy, Dandelion, Roses, Sunflowers, and Tulips using transfer learning (MobileNetV2) and the tf_flowers dataset.

📌 Features

✅ Dataset from tensorflow_datasets

✅ Preprocessing and batching using tf.data

✅ Trained with MobileNetV2 (transfer learning)

✅ Evaluated using accuracy and confusion matrix

✅ Works seamlessly in Google Colab

📂 Dataset

Source: TFDS - tf_flowers

Contains over 3,600 flower images labeled into 5 classes.

🧠 Model Architecture

Base: MobileNetV2 (pretrained on ImageNet)

Classifier Head:

- Global Average Pooling

- Dense Layer (128 ReLU)

- Output Layer (5-class softmax)

- Loss: Sparse Categorical Crossentropy

- Optimizer: Adam

📊 Evaluation

Achieved ~90%+ accuracy on validation set

Confusion matrix reveals strong performance, with minor overlap between visually similar classes.


🖼️ Sample Prediction


🌸 Prediction: Sunflower (Confidence: 97.5%)

✅ Requirements

- TensorFlow

- TensorFlow Datasets

- Matplotlib

- scikit-learn (for confusion matrix)
