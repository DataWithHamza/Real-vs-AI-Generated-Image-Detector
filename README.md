# 🤖 Real vs AI-Generated Image Detector

A Deep Learning-based web application that detects whether an uploaded image is **Real (Authentic)** or **AI-Generated** (created by generative AI models like Midjourney, DALL-E, or Stable Diffusion). 

The project uses a Convolutional Neural Network (CNN) model trained on the **CIFAKE dataset**, achieving a high validation accuracy. It is integrated with a user-friendly **Streamlit** web interface and deployed on **Hugging Face Spaces**.

---

## 🚀 Live Demo
You can try the live web application here:
👉 **[Hugging Face Space Live App](https://huggingface.co/spaces/hamza-3120/real-vs-ai-detector)**

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

💻 Technologies Used

Frontend: Streamlit 🎈

Deep Learning Framework: TensorFlow / Keras 🧠

Image Processing: Pillow (PIL) 🖼️

Numerical Operations: NumPy 🔢

Deployment Platform: Hugging Face Spaces / Docker 🐳

🔧 Installation & Local Setup
To run this project locally, follow these steps:

Clone the repository:

Bash
git clone [https://github.com/DataWithHamza/Real-vs-AI-Image-Detector.git](https://github.com/DataWithHamza/Real-vs-AI-Image-Detector.git)
cd Real-vs-AI-Image-Detector
Install dependencies:

Bash
pip install -r requirements.txt
Run the Streamlit app:

Bash
streamlit run src/app.py

👥 Author
Hamza (@DataWithHamza)
