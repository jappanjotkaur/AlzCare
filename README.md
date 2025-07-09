# 🧠 AlzCare – Smart Assistance System for Alzheimer’s Patients

AlzCare is an AI-powered real-time assistance system designed to support elderly individuals, especially those suffering from Alzheimer’s disease. The system monitors daily human activities using webcam input, detects anomalies like falls or prolonged inactivity, and sends instant alerts to caregivers or family members.

🎥 **Demo video is attached in the repository to showcase the working of the complete system.**

---

## 📌 Features

- 👀 Real-Time Human Activity Monitoring using MediaPipe Pose  
- 🧠 AI-Based Activity Classification using CNN-LSTM  
- 🚨 Fall Detection and Anomaly Alerting  
- 📡 Live Video Streaming (Flask-based)  
- 📲 Flutter-Based Mobile UI  
- ⚠️ Alert Notification System via SMS or UI popups  
- 🔐 Secure and lightweight – ideal for home or healthcare center use  

---

## 🏗️ Tech Stack

| Component            | Technology              |
|---------------------|-------------------------|
| Pose Estimation     | MediaPipe Pose          |
| Deep Learning Model | CNN-LSTM (TensorFlow/Keras) |
| Backend             | Python, Flask           |
| Frontend Interface  | Flutter (Dart)    |
| Video Handling      | OpenCV                  |
| Notifications       | SMTP / Twilio API       |

---

## 📁 Project Structure

```
AlzCare/
│
├── Alzcare Project/
│   ├── model/                   # CNN-LSTM model files
│   ├── mediapipe_activity.py    # Pose detection and activity classification
│   ├── app.py                   # Flask app for live video and alerts
│   ├── gui/                     # Kivy GUI interface
│   ├── flutter_ui/              # 📱 Flutter UI with individual Dart files
│   │   ├── main.dart
│   │   ├── home.dart
│   │   ├── alert_screen.dart
│   │   └── ... (other UI components)
│   ├── utils/                   # Helper functions and utilities
│   └── requirements.txt  
│          
├── demo_video.mp4   # 📹 Attached demo video showing full functionality
└── README.md
```

> 📌 **Note:** The `flutter_ui/` folder under `Alzcare Project` contains the complete Flutter-based mobile application. All Dart files are individually named and reflect the screen/component structure clearly. These align with the modular architecture of the project.

---

## ⚙️ Installation

### 🐍 Backend Setup

1. **Clone the Repository**
```bash
git clone https://github.com/riyakansal04/AlzCare.git
cd "AlzCare/Alzcare Project"
```

2. **Create Virtual Environment (Optional)**
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

3. **Install Python Dependencies**
```bash
pip install -r requirements.txt
```

4. **Run Backend Server**
```bash
python app.py
```

---

### 📱 Flutter UI Setup

1. Navigate to the Flutter UI directory:
```bash
cd "AlzCare/Alzcare Project/flutter_ui"
```

2. Get dependencies and run:
```bash
flutter pub get
flutter run
```

---

## 🧪 AI Model

- Model Type: CNN + LSTM  
- Framework: TensorFlow/Keras  
- Input: 33 Pose Landmarks per frame (via MediaPipe)  
- Output: Activity Classes – Walking, Sitting, Standing, Falling, Heartstroke, Coughing, Headache


---


## 👩‍💻 Authors

- **Jappanjot Kaur** – AI & System Architecture  
- **Riya Kansal** – AI/ML Developer & Flutter Integration  

GitHub: [https://github.com/riyakansal04](https://github.com/riyakansal04)  

---

## 📞 Contact

For collaboration or demo requests, feel free to reach out:  
📧 riyakansal174@gmail.com
📧jappanjotkaur2004@gmail.com
🔗 [GitHub Repository](https://github.com/riyakansal04/AlzCare)
