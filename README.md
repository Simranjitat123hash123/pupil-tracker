# 👁️ Pupil Dilation Tracker

**A Web-Based Eye-Tracking Application for Intercultural Engagement Analytics**  
Part of an ongoing **PhD Research Prototype**.

---

## 🌐 Live Applications

| Application | Description | Live Link |
|--------------|--------------|------------|
| 🎓 **Student App** | Captures pupil dilation in real-time using webcam, :contentReference[oaicite:0]{index=0}, and :contentReference[oaicite:1]{index=1}. | [Open Student App →](https://simranjitat123hash123.github.io/pupil-tracker/student.html) |
| 🧑‍🏫 **Teacher Dashboard** | Displays live student engagement data from :contentReference[oaicite:2]{index=2}. | [Open Teacher Dashboard →](https://simranjitat123hash123.github.io/pupil-tracker/teacher.html) |

---

## 🧩 Project Overview

The **Pupil Dilation Tracker** measures student engagement by analyzing iris and pupil dilation through the webcam in real time.  
It integrates:
- **:contentReference[oaicite:3]{index=3}** for facial landmark detection  
- **:contentReference[oaicite:4]{index=4}** for pupil segmentation  
- **:contentReference[oaicite:5]{index=5}** for storing live session data  
- A teacher dashboard to visualize aggregated engagement data  

---

## 🧠 Research Context

This system is developed as part of an **Intercultural Engagement Analytics** framework, studying how cognitive and affective responses can be tracked using physiological indicators like pupil dilation during online learning sessions.

---

## ⚙️ Features

### 🎓 Student Interface
- Real-time pupil and iris detection using webcam
- Auto-calibration for baseline measurement
- Displays normalized dilation and % change
- Securely uploads to Firebase every second
- Works in most modern browsers

### 🧑‍🏫 Teacher Dashboard
- Live view of connected students
- Shows minutes where dilation ≥ 25% (engaged) vs < 25% (less engaged)
- Auto-refresh every few seconds
- Exportable data to Excel (XLSX)
- Reset and refresh options for sessions

---

## 🛠️ Technology Stack

| Category | Tools Used |
|-----------|-------------|
| Frontend | HTML5, CSS3, JavaScript (ES6) |
| Vision Processing | :contentReference[oaicite:6]{index=6}, :contentReference[oaicite:7]{index=7} |
| Database | :contentReference[oaicite:8]{index=8} |
| Hosting | :contentReference[oaicite:9]{index=9} |
| Export | :contentReference[oaicite:10]{index=10} (XLSX.js) |

---

## 🚀 Setup & Deployment

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Simranjitat123hash123/pupil-tracker.git
cd pupil-tracker
```

### 2️⃣ Open Student or Teacher App
Simply open these in a browser:
```
student.html
teacher.html
```

### 3️⃣ Firebase Configuration
Make sure your Firebase database rules (for testing) are open:
```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

Replace your Firebase config inside both HTML files if needed.

---

## 📊 Data Flow
```text
Student (Webcam) 
   ↓ 
FaceMesh + OpenCV
   ↓ 
Normalized Dilation %
   ↓ 
Firebase Realtime Database
   ↓ 
Teacher Dashboard (Aggregated Engagement)
```

---

## 📈 Example Screenshot
*(You can add your own screenshots later)*

![Pupil Tracker Interface Screenshot](https://user-images.githubusercontent.com/example/screenshot.png)

---

## 📜 License
This project is created as part of academic research and is not intended for commercial use.  
© 2026 Simranjit Singh — All Rights Reserved.

---

## 📬 Contact
**Researcher:** Simranjit Singh  
**Email:** (add your research email if you wish)  
**GitHub:** [Simranjitat123hash123](https://github.com/Simranjitat123hash123)
