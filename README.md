# Deepfake Detection System Using MobileNetV2 & Audio Forensics

## 📌 Overview

This project is a multimodal Deepfake Detection System that identifies manipulated (fake) videos by analyzing both visual and audio content. The system combines deep learning techniques for video frame analysis and audio forensics to improve detection performance.

The visual module uses MobileNetV2 to extract spatial features from video frames, while the audio module uses LSTM to analyze audio features extracted from the video's soundtrack. The system classifies media as either **Real** or **Fake**.

---

## 🎯 Features

- Detects Deepfake videos using deep learning
- Video analysis using MobileNetV2
- Audio analysis using LSTM
- Face extraction from video frames
- Automatic frame extraction
- Audio feature extraction using MFCC
- Real/Fake prediction with confidence score
- User-friendly prediction interface

---

## 🏗️ System Architecture

### Video Module
1. Upload video
2. Extract frames
3. Detect and crop faces
4. Resize images
5. Extract features using MobileNetV2
6. Classify as Real or Fake

### Audio Module
1. Extract audio from video
2. Preprocess audio
3. Extract MFCC features
4. Analyze using LSTM
5. Classify as Real or Fake

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- MobileNetV2
- LSTM
- Librosa
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Flask (for deployment)

---

## 📂 Project Structure

```
Deepfake-Detection-System/
│
├── dataset/
│   ├── video/
│   │   ├── real/
│   │   └── fake/
│   └── audio/
│       ├── real/
│       └── fake/
│
├── models/
│   ├── mobilenetv2_video_model.keras
│   ├── lstm_audio_model.keras
│
├── notebooks/
│   ├── Video_Training.ipynb
│   ├── Audio_Training.ipynb
│
├── app.py
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 📊 Dataset

### Video Dataset
- Real Videos
- Fake Videos

### Audio Dataset
- Real Audio
- Fake Audio

The dataset is preprocessed by:
- Frame extraction
- Face detection
- Image resizing
- Audio extraction
- MFCC feature extraction

---

## 🧠 Deep Learning Models

### Video Detection
- MobileNetV2
- Transfer Learning
- Binary Classification

### Audio Detection
- LSTM Network
- MFCC Features
- Binary Classification

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Deepfake-Detection-System.git
```

Go to project directory:

```bash
cd Deepfake-Detection-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python app.py
```

---

## 📈 Workflow

```
Video Input
      │
      ▼
Frame Extraction
      │
      ▼
Face Detection
      │
      ▼
MobileNetV2
      │
      ▼
Video Prediction
      │
      ├─────────────┐
      ▼             │
Audio Extraction    │
      │             │
      ▼             │
MFCC Features       │
      │             │
      ▼             │
LSTM Model          │
      │             │
      └──────┬──────┘
             ▼
      Final Prediction
        (Real/Fake)
```

---

## 📌 Future Improvements

- Real-time webcam detection
- Attention-based deep learning models
- Transformer-based architectures
- Support for longer videos
- Cloud deployment
- Mobile application integration

---

## 👨‍💻 Author

**Syed Israr Hussain**

BS Software Engineering

Hazara University

Interests:
- Data Science
- Data Analysis
- Artificial Intelligence
- Deep Learning
- Computer Vision

---

## 📄 License

This project is developed for academic and research purposes.
