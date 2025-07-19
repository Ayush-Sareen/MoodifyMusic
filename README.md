# 🎵 MoodifyMusic - Emotion-Based Music Recommender 🎭🎶

MoodifyMusic is a real-time emotion detection system that recommends songs based on your current mood. It uses your facial and hand gestures via your webcam to predict emotions with a machine learning model and recommends matching songs from YouTube.

---

## 🚀 Features

- 🎥 Real-time webcam-based emotion detection
- 🧠 Deep learning model trained on landmark data (face + hands)
- 🎯 Predicts emotions like happy, sad, angry, etc.
- 🔗 Recommends music based on:
  - Detected emotion
  - Selected language
  - Optional singer input
- 🌐 Built using Streamlit + WebRTC

---

## 🎬 Demo

> 📺 **Watch the Live Demo Below**  
> *(Click the video or open it in YouTube)*

[![MoodifyMusic Demo](https://img.youtube.com/vi/jsJrREv9lyY/0.jpg)](https://www.youtube.com/watch?v=jsJrREv9lyY)

---

## 🛠️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/MoodifyMusic.git
   cd MoodifyMusic
Install dependencies:

```bash
pip install -r requirements.txt
```
Run the app:

```bash
streamlit run music.py
```
📂 Project Structure
```bash
MoodifyMusic/
├── liveEmoji        # Folder for training the model 
├── music.py                  # Streamlit app for real-time emotion detection
├── model.h5                # Trained Keras model
├── labels.npy              # Emotion labels
├── emotion.npy             # Temp file to store detected emotion
├── requirements.txt
└── README.md
```
📦 Dependencies
```txt
streamlit
streamlit-webrtc
opencv-python
mediapipe
tensorflow
numpy
av
```
Install using:

```bash
pip install -r requirements.txt
```
📸 How It Works
Webcam captures your facial and hand movements.

Mediapipe extracts landmark positions.

Pre-trained neural network predicts your emotion.

You click “Recommend me songs” — it opens a YouTube search like:

```arduino
https://www.youtube.com/results?search_query=English+happy+song+Ed+Sheeran
```
