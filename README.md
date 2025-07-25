# 🎙️ Multilingual Speech Emotion Analyzer (Offline Compatible)

This is a powerful **AI-based speech analytics web application** that performs:
- 🎧 **Speech Transcription** (up to 40 minutes)
- 🌍 **Language Translation** (multi-language to English)
- 💬 **Sentiment Analysis** (emotion detection with explanation)
- ⭐ **Star Rating System** (based on mood intensity)

Designed for **local or offline execution**, the app ensures minimal internet dependency while maintaining **high accuracy**.

---

## 🔧 Features

| Feature                | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| ✅ Whisper ASR         | Uses OpenAI's Whisper model for accurate transcription                      |
| ✅ Offline Translation | Switches to offline model to avoid internet-based delays                    |
| ✅ Emotion Analysis    | Uses VADER + Rule-Based NLP to identify precise emotional tones             |
| ✅ Explanation Panel   | Describes mood and sentiment contextually                                   |
| ✅ Star Rating         | Based on compound score (from 1⭐ to 5⭐)                                     |
| ✅ Fast Runtime        | Optimized for large audios (up to 40 mins) in minimal time                  |
| ✅ Gradio UI           | Clean user interface for input/output separation                            |

---

## 🚀 Technologies Used

- 🧠 Whisper (Local ASR Model)
- 🔤 MarianMT / NLLB / SentencePiece (Offline Translators)
- 📊 NLTK & Rule-Based NLP
- 🧪 VADER SentimentIntensityAnalyzer
- 🎛️ Gradio for Web UI
- 🐍 Python 3.11
- 🧰 Torch, Torchaudio

---

## 🖼️ Output Interface

| Section        | Output Example                     |
|----------------|------------------------------------|
| 🎧 Transcription | `"Hello, how are you doing today?"` |
| 🌐 Translation   | `"Hello, how are you doing today?"` |
| 💬 Sentiment     | `"Positive"`                       |
| 📘 Explanation   | `"The sentence indicates a friendly and calm tone."` |
| ⭐ Rating        | `⭐⭐⭐⭐⭐`                             |

---

## 📥 How to Run (Google Colab / Local)

### 🔹 For Google Colab
1. Open Colab and upload your `.wav`/`.mp3` file
2. Install dependencies:
```bash
!pip install git+https://github.com/openai/whisper.git gradio torchaudio nltk transformers sentencepiece
