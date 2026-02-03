# Fashion-MNIST-Image_Classification
https://colab.research.google.com/drive/1eZaY0wNWf5qE90qUErrOLB4rg7D_ragF?usp=sharing

1. What is the Fashion MNIST dataset?**

The **Fashion MNIST dataset** is a collection of **70,000 grayscale images** of clothing items, each sized **28×28 pixels**.
It contains **10 different fashion categories** such as T-shirts, trousers, shoes, and bags.
The dataset is commonly used to **train and test machine learning models**, especially as a more challenging replacement for the original MNIST digit dataset.

---

2. Why do we normalize image pixel values before training?**

We normalize pixel values to **scale them from 0–255 down to 0–1**.
This helps the neural network **train faster and more efficiently** by keeping numerical values small and consistent.
Normalization also improves **model stability and accuracy** during training.

---

3. List the layers used in the neural network and their functions.**

* **Flatten layer**
  Converts the 2D image (28×28) into a 1D array so it can be processed by dense layers.

* **Dense layer (128 neurons, ReLU activation)**
  Learns important features from the image and introduces non-linearity to improve learning.

* **Dense output layer (10 neurons)**
  Produces one output value for each clothing class, representing the model’s confidence for each category.

---

4. What does an epoch mean in model training?**

An **epoch** is **one complete pass through the entire training dataset** during model training.
Each epoch allows the model to update its weights and improve predictions.
Training for multiple epochs helps the model **learn patterns more effectively**.

---

5. Compare the predicted label and actual label for the first test image.**

The **predicted label** is the class chosen by the model based on the highest probability.
The **actual label** is the true class provided in the dataset.
If both labels match, the prediction is **correct**; if they differ, the model made a **misclassification**.

---

6. What could be done to improve the model’s accuracy?**

* Increase the **number of training epochs**
* Add more **hidden layers or neurons**
* Use **Dropout layers** to reduce overfitting
* Apply **data augmentation**
* Tune hyperparameters such as **learning rate or batch size**
* Use a **Convolutional Neural Network (CNN)** instead of a basic dense model
