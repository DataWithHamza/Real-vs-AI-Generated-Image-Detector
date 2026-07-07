# 🤖 Real vs AI-Generated Image Detector
🧠 A Deep Learning-based web application powered by a Convolutional Neural Network (CNN) trained on the CIFAKE dataset to classify images as Real or AI-Generated with 91.82% accuracy. Built using TensorFlow and Streamlit, and deployed live on Hugging Face Spaces. 🚀

A web application that detects whether an uploaded image is **Real (Authentic)** or **AI-Generated** (created by generative AI models like Midjourney, DALL-E, or Stable Diffusion). 

The project uses a Convolutional Neural Network (CNN) model trained on the **CIFAKE dataset**, achieving a high validation accuracy. It is integrated with a user-friendly **Streamlit** web interface and deployed on **Hugging Face Spaces**.

---

## 🚀 Live Demo
You can try the live web application here:
👉 **[https://huggingface.co/spaces/hamza-3120/real-vs-ai-detector]**

---

## 📊 Model Performance & Metrics
The CNN model was trained over 10 epochs on the CIFAKE dataset and achieved the following results:

| Metric | Training Set | Validation Set |
| :--- | :--- | :--- |
| 🎯 **Accuracy** | 93.68% | 91.82% |
| 📉 **Loss** | 0.1601 | 0.2114 |

* **Classification Threshold:** Optimized at `0.22` based on specific model confidence score distributions to ensure precise distinction between Real and AI images.

---

## 🛠️ Features
* 📷 **Image Upload:** Supports `.jpg`, `.jpeg`, and `.png` formats.
* 📊 **Confidence Score:** Displays the exact probability score from the model.
* 🎨 **Interactive UI:** Clean feedback with distinct visual indicators (Success/Error blocks).

---

## 📦 Project Structure
```text
├── src/
│   ├── app.py                     # Main Streamlit application code
│   └── real_vs_ai_model.keras     # Trained TensorFlow/Keras model file
├── requirements.txt               # Dependencies list
└── README.md                      # Project documentation
