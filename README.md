# animal-classifier-trained
An image classification model trained via Teachable Machine and validated on Google Colab to classify dogs, cats, and rabbits with high accuracy.

# 🐾 Animal Classification Model using Teachable Machine & Keras

An end-to-end computer vision project focused on image classification. The model is trained to recognize and distinguish between three different animal categories (Dog, Cat, and Rabbit) using deep learning techniques. 

The core model was trained via **Teachable Machine**, and its performance and inference accuracy were verified inside **Google Colab** using TensorFlow and Keras.

---

## 🚀 Project Overview

The workflow of this project is divided into two main phases to ensure seamless deployment and high prediction accuracy:
1. **Training Phase:** Gathering sample datasets, training the classification layers, and exporting the trained weights as a Keras architecture (`.h5` format).
2. **Verification & Inference Phase:** Developing a Python script hosted on Google Colab to load the Keras model, process new test images, and output the model's exact prediction along with its confidence score.

---

## 📊 Workflow & Results

### 1. Model Training
* **Platform Used:** Google's Teachable Machine.
* **Target Classes:** 
  * `dog`
  * `cat`
  * `rabbit`
* **Output Artifacts:** The trained model was exported as `keras_model.h5` along with its corresponding class index file `labels.txt`.

### 2. Validation on Google Colab
The model's deployment logic was verified by uploading the Keras file into a Colab notebook and running inference using `TensorFlow` and `Pillow (PIL)`. 

When evaluated against a fresh test image of a dog, the model demonstrated outstanding generalization capability, producing a near-perfect confidence metric:
* **Predicted Class:** `dog`
* **Confidence Score:** `0.99996495` (~99.99% certainty)

---

## 🛠️ Installation & Usage

To run the inference script locally or within your own cloud environment, ensure you have the required dependencies installed:

```bash
pip install tensorflow pillow numpy
