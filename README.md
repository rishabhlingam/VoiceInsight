# 🎙️ VoiceInsight

**VoiceInsight** is a simple web app that lets you **record your voice**, **upload the audio**, and get an **AI-generated transcription and sentiment analysis** using Google’s **Gemini model**.

---

## ⚙️ Features
- Record audio directly in your browser  
- Automatically transcribe speech using Gemini  
- Get sentiment analysis (Positive / Neutral / Negative)  
- View and play all past recordings  
- Ready to deploy on Google Cloud Run or Render  

---

## 🛠️ Tools Used
- **Frontend:** HTML, JavaScript (MediaRecorder API)  
- **Backend:** Flask (Python)  
- **AI Model:** Google Vertex AI – Gemini 1.5 Pro  
- **Deployment:** Gunicorn + Procfile  
- **Other:** Jinja2, datetime, os  

---

## 🚀 How to Run
Clone the repo:  
`git clone https://github.com/<your-username>/VoiceInsight.git`  
`cd VoiceInsight`

Install dependencies:  
`pip install -r requirements.txt`

Set up Google Cloud:  
`export GOOGLE_CLOUD_PROJECT="your-project-id"`  
`gcloud auth application-default login`

Run the app:  
`python main.py`

Open your browser and go to **http://127.0.0.1:8080**

---

## 🧠 How It Works
1. You record audio using your browser’s microphone.  
2. The app saves it and sends it to **Gemini 1.5 Pro**.  
3. Gemini returns a **transcription** and **sentiment**.  
4. Both results are saved and displayed on the webpage.
