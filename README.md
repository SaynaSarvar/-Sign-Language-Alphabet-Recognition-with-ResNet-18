### 🤖 Hand Gesture Recognition

This project uses **PyTorch** and **Fine-Tuning** to build a deep learning model that recognizes American Sign Language (ASL) letters from hand images. I developed this project after completing a PyTorch course to solidify my understanding of key concepts.

---

### 📚 Dataset

The model is trained and evaluated on the **Sign Language MNIST dataset** from Kaggle. This dataset contains 28x28 pixel images of hand gestures for 24 letters of the English alphabet (excluding `J` and `Z`).

---

### 🧠 Model Architecture & Fine-Tuning

* **Base Model:** A pre-trained **ResNet-18** model, originally trained on the ImageNet dataset, serves as the backbone.
* **Method:** I apply the **Fine-Tuning** technique to adapt the ResNet-18 model for sign language recognition.
* **Layer Freezing:** To optimize training, the initial layers of ResNet-18 (`conv1`, `layer1`, `layer2`, `layer3`) are frozen, ensuring over **3 million parameters** remain unchanged during training. Only the deeper layers and the final fully connected layer are trained.

---

### ✅ Results

* **Accuracy:** The model achieved an accuracy of **99.84%** on the test set.
* **F1-Score:** The final F1-Score was **99.84%**, indicating a high level of precision and recall.
