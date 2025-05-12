# 🎥 Multimodal Emotion Detection System

This project implements a **Multimodal Emotion Detection System** that analyzes both **facial expressions** and **audio features** from video input to detect emotional states. It combines **computer vision**, **audio signal processing**, and **simple rule-based classification** to predict an overall emotion.

---

## 🔍 Features

- **Facial Emotion Recognition** using DeepFace on sampled video frames.
- **Audio Emotion Recognition** using MFCC, ZCR, RMSE, and other features via `librosa`.
- **Multimodal Fusion** logic to combine visual and vocal cues for robust emotion analysis.
- **Interactive Visualizations** using `matplotlib` for both audio and facial emotion insights.
- Works with video uploads in a **Google Colab** environment.

---

## 🧠 How It Works

1. **Upload a video file** via Google Colab.
2. **Extract facial frames** and detect dominant emotions using DeepFace.
3. **Extract audio** from the video and analyze it using spectral features.
4. **Classify audio emotion** using simple thresholds on energy and ZCR.
5. **Fuse visual and audio insights** to determine a final emotion.
6. **Visualize** both intermediate and final results with charts.

---

## 📁 Requirements

- Python 3.x  
- Libraries:
  - `opencv-python`
  - `librosa`
  - `deepface`
  - `moviepy`
  - `matplotlib`
  - `numpy`
  - `google.colab` (for file upload in Colab)
  - `IPython.display`

---

## 🚀 Getting Started

Run this notebook in **Google Colab** for best compatibility.

```python
# Clone or upload the script, then run:
from your_script_name import MultimodalEmotionDetector

detector = MultimodalEmotionDetector()
detector.run_analysis()
```

> ⚠️ Note: DeepFace uses pre-trained models and may require initial downloads.

---

## 📊 Output

- Dominant facial emotions over frames
- Classified audio emotion
- Final fused emotion
- Bar charts and audio spectrograms

---

## 📌 Use Case

This is an ideal tool for research or academic projects in:
- Affective computing
- Human-computer interaction
- Behavioral analysis

---

## 📄 License

This project is for educational and research purposes. Please check individual library licenses for usage in commercial settings.
