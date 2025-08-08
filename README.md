# 🎤 Sound Activity Detector 

A simple web app that uses your device's microphone to detect unusual sound activity in real-time — built with HTML, CSS, and vanilla JavaScript.  
This is simple, beginner-like audio code.

## 🚀 Features
- 🎧 **Live microphone monitoring** using `navigator.mediaDevices.getUserMedia`
- 🔍 **Volume detection algorithm** to flag unusual sound spikes

---

## 🛠️ How It Works

1. **Microphone Access**  
   Uses the Web Audio API (`AudioContext`, `AnalyserNode`) to capture real-time audio input.

2. **Volume Detection**  
   - Captures waveform data via `getByteTimeDomainData`
   - Calculates the RMS (Root Mean Square) of the audio signal
   - Triggers an alert message if the volume exceeds a threshold
