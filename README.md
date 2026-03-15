# Content-Based Image Retrieval (CBIR) using VGG16, PCA, and t-SNE

## 📌 Overview
This project implements a Content-Based Image Retrieval (CBIR) system. Unlike traditional text-based search methods, this vision-based approach uses deep learning to understand and retrieve images based on visual similarity (such as color, texture, and form). 

The system extracts high-dimensional image embeddings using a pre-trained **VGG16** model, applies dimensionality reduction techniques (**PCA** and **t-SNE**) to visualize the data, and utilizes **Cosine Similarity** to find and return the closest matching artwork or image from the dataset.

## 🚀 Features
* **Feature Extraction:** Utilizes the VGG16 Convolutional Neural Network (CNN) without the top classification layers to extract rich, 512-dimensional feature vectors from images.
* **Dimensionality Reduction & Visualization:** * Implements **PCA (Principal Component Analysis)** for global variance-based dimensionality reduction.
  * Implements **t-SNE (t-Distributed Stochastic Neighbor Embedding)** to uncover hidden non-linear patterns and visual clusters.
* **Image Retrieval:** Computes Cosine Similarity between the uploaded query image's embedding and the dataset embeddings to retrieve the visually closest match.

## 🛠️ Technologies Used
* **Language:** Python
* **Deep Learning Framework:** TensorFlow / Keras (VGG16)
* **Machine Learning Library:** Scikit-Learn (PCA, t-SNE, Cosine Similarity)
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Google Colab / Jupyter Notebook

## ⚙️ How It Works
1. **Preprocessing:** Input images are resized to 224x224 and preprocessed to fit the VGG16 input format.
2. **Embedding Generation:** The pre-trained VGG16 model generates a feature vector for each image in the corpus.
3. **Visualization:** The 512-dimensional embeddings are reduced to 2D using PCA and t-SNE, allowing for scatter plot visualization of the image relationships.
4. **Search Query:** A new test image is uploaded and processed through the same pipeline.
5. **Matching:** The system calculates the cosine similarity and displays the query image side-by-side with its closest match from the database.




