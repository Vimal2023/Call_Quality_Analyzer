# 🎧 Call Quality Analyzer

This repository contains my submission for the **Voice AI Startup Assignment**.  
The project is built in **Google Colab** and analyzes sales call recordings to extract useful insights.

---

## 🚀 Features
- ✅ Talk-time ratio (percentage each person spoke)  
- ✅ Number of questions asked  
- ✅ Longest monologue duration  
- ✅ Call sentiment (positive / negative / neutral)  
- ✅ One actionable insight for improvement  
- 🎯 Bonus: Speaker diarization (identify Sales Rep vs Customer)

---

## ⚙️ Tech Stack
- **Python**
- **Google Colab**
- **OpenAI Whisper** – Speech-to-text  
- **HuggingFace Transformers** – Sentiment analysis  
- **Pyannote / WhisperX** – Speaker diarization  
- **yt-dlp** – Extract audio from YouTube  

---

## 📊 Approach (Short Explanation)
My approach uses **speech-to-text + text analysis**.  
I first extract the call audio and transcribe it using **Whisper**, which handles poor-quality audio.  
Using timestamps, I calculate talk-time ratio and longest monologue. Questions are counted by detecting `?` and interrogatives. Sentiment is identified with HuggingFace transformers. Finally, I generate an **actionable insight** to improve sales interactions.  

For the **bonus task**, I used speaker diarization with Pyannote/WhisperX to differentiate between the sales rep and the customer.  

The system runs under **30 seconds** on the free Colab tier.  

---
## 📂 Repository Structure
📦 Call_Quality_Analyzer
┣ 📜 Call_Quality_Analyzer.ipynb # Main Colab notebook
┣ 📜 README.md # Project documentation

---

---

## ▶️ How to Run
1. Open the notebook in Google Colab  
2. Run all cells in order (install → import → download audio → transcription → analysis)  
3. Results will be printed at the end  

---

## 📌 Test File
- Assignment test file: [YouTube Call Recording](https://www.youtube.com/watch?v=4ostqJD3Psc)

---

## 👤 Author
**Vimal Anand** 

