# Audio Classification with YAMNet

This project uses [YAMNet](https://tfhub.dev/google/yamnet/1), a pretrained deep learning model from TensorFlow Hub, to classify and interpret audio files. The model is capable of identifying sound events and is extended here to attempt classification into human voice, human voicemail, and machine voicemail.

## 🔍 Features

- Loads `.wav` audio files and preprocesses them.
- Runs predictions using the YAMNet model.
- Displays top predicted audio classes and confidence scores.
- Attempts to classify the audio into:
  - Human voice
  - Human voicemail
  - Machine voicemail or alert

## 🧠 Model

- **YAMNet** is trained on the [AudioSet](https://research.google.com/audioset/) dataset from Google.
- Predicts 521 audio event classes.

## 📁 File Structure


## ▶️ How to Use

1. **Clone the repository**:

```bash
git clone git@github.com:haroon423/audio-classification-yamnet.git
cd audio-classification-yamnet

pip install tensorflow tensorflow_hub numpy scipy matplotlib

python predict_voicemail.py

Top predicted classes and scores for 'your_audio.wav':
Speech: 0.856
Silence: 0.137
Speech synthesizer: 0.027
Narration, monologue: 0.012
Conversation: 0.005
Detected: Human voice


---

Paste the above into your `README.md` file, and it will render cleanly on GitHub with proper markdown formatting and structure. Let me know if you want to include a demo audio or a sample result JSON/CSV too.
