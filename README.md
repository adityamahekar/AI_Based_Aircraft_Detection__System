
# ✈️ AI-Based Aircraft Recognition System
**Aircraft Detection using YOLOv8 and Classification using ResNet-50**

[![Google Drive](https://img.shields.io/badge/Google%20Drive-Full%20Project-4285F4?style=for-the-badge&logo=google-drive&logoColor=FFFFFF)](https://drive.google.com/drive/folders/149i_iHdHYb1TVz3OH6jZMLhLpTInKpq3)

---

## 📌 Project Overview

**AI-based Aircraft Recognition System** capable of detecting aircraft in **images, videos, and real-time camera feeds** and identifying their type automatically.

# Dashboard & Results

| **Dashboard** | **ATR-72** |
|---------------|------------|
| ![Dashboard](https://raw.githubusercontent.com/arun0180/AI-Based-AircraftRecognition-System/main/dashboard.jpg) | ![ATR-72](https://raw.githubusercontent.com/arun0180/AI-Based-AircraftRecognition-System/main/ATR_72_29.jpg) |

| **MiG-29** | **Su-30** |
|------------|-----------|
| ![MiG-29](https://raw.githubusercontent.com/arun0180/AI-Based-AircraftRecognition-System/main/MiG-29_80.jpg) | ![Su-30](https://raw.githubusercontent.com/arun0180/AI-Based-AircraftRecognition-System/main/Su-30_24.jpg) |

| **MQ-9 Reaper** | **Su-30** |
|-----------------|-----------|
| ![MQ-9 Reaper](https://raw.githubusercontent.com/arun0180/AI-Based-AircraftRecognition-System/main/MQ-9_Reaper_Drone_7.jpg) | ![Su-30](https://raw.githubusercontent.com/arun0180/AI-Based-AircraftRecognition-System/main/Su-30_25.jpg) |
**System Architecture:**
```
YOLOv8 (Detection) → Bounding Boxes → ResNet-50 (Classification) → Aircraft Type + Confidence
```

### Applications
- Airport surveillance
- Airspace monitoring
- Defense and security systems
- UAV and drone tracking
- Aviation research and analytics

---

## 🚀 Features

- ✔ Aircraft detection using **YOLOv8**
- ✔ Aircraft classification using **ResNet-50**
- ✔ Image input support
- ✔ Video input support
- ✔ Real-time webcam detection
- ✔ Web-based interface using **Flask**
- ✔ Modular architecture (detection + classification pipeline)

---

## 🧠 Models Used

### 1️⃣ YOLOv8 (Detection Model)
- Detects aircraft in an image
- Outputs bounding box coordinates
- Provides confidence score
- Fast and suitable for real-time applications

### 2️⃣ ResNet-50 (Classification Model)
- Deep Convolutional Neural Network
- Uses transfer learning
- Classifies cropped aircraft images
- Handles fine-grained aircraft differences

---

## 📂 Project Structure

```
AI-Aircraft-Recognition-System/
│
├── app.py
├── scripts/
│   ├── train_detector.py
│   ├── train_classifier.py
│   ├── recognize_image.py
│   └── detect_video.py
│
├── models/               # Model architecture files
├── test_images/          # Sample test images
├── data.yaml            # YOLO dataset configuration
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 📊 Dataset Information

**Aircraft images collected from:**
- FGVC-Aircraft Dataset
- FAIR1M Dataset
- UCAS-AOD Dataset
- Public aviation image sources

**Dataset includes:**
- Commercial aircraft
- Military aircraft
- UAV types
- Different angles and lighting conditions

**Dataset split:**
- Training set
- Validation set
- Testing set

**Annotation:** LabelImg in YOLO format

---

## ⚙️ Installation Guide

### 🔹 Step 1: Clone Repository
```bash
git clone https://github.com/arun0180/AI-Aircraft-Recognition-System.git
cd AI-Aircraft-Recognition-System
```

### 🔹 Step 2: Create Virtual Environment (Recommended)
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# Linux/Mac
source venv/bin/activate
```

### 🔹 Step 3: Install Requirements
```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run the Project

### 🔹 Run Web Application
```bash
python app.py
```
**Open browser:** http://127.0.0.1:5000

### 🔹 Train Models
```bash
python scripts/train_detector.py      # YOLOv8 Detector
python scripts/train_classifier.py    # ResNet Classifier
```

### 🔹 Run Detection
```bash
python scripts/recognize_image.py     # Image detection
python scripts/detect_video.py        # Video detection
```

---

## 📈 Performance Metrics

**Evaluated using:**
- Accuracy
- Precision
- Recall
- F1-score
- mAP (mean Average Precision)
- Confusion Matrix

**Results:**
- Accurate detection in complex backgrounds
- Reliable classification across multiple aircraft types
- Real-time performance with GPU support

---

## 💻 Technologies Used

```
-  Python
-  PyTorch
-  Ultralytics YOLOv8
-  OpenCV
-  NumPy
-  Matplotlib
-  Flask
```

---

## 🔥 Key Advantages

- **End-to-end aircraft recognition**
- **Real-time capability**
- **Scalable architecture**
- **Modular detection + classification design**
- **Easy deployment**

---

## ⚠️ Limitations

- Performance may reduce for very small aircraft
- Visually similar aircraft may cause minor confusion
- Real-time performance depends on hardware

---

## 🔮 Future Enhancements

- Add aircraft tracking (DeepSORT)
- Expand dataset with more aircraft types
- Deploy on edge devices (Jetson Nano)
- Integrate satellite image support
- Add Explainable AI (Grad-CAM visualization)

---

## 📌 Applications

- **Airport security monitoring**
- **Airspace surveillance**
- **Defense monitoring systems**
- **UAV monitoring**
- **Aviation analytics**

---

## 👥 Development Team

**Mini Project**  
**Department of Computer Science and Engineering**  
**BMS Institute of Technology & Management**

| Contributor | LinkedIn |
|-------------|----------|
| Aditya Mahekar | [Profile](https://www.linkedin.com/in/aditya-mahekar/) |
| Arun Biradar | [Profile](https://www.linkedin.com/in/arun-biradar01/) |
| Abhishek Ireddy | [Profile](https://www.linkedin.com/in/abhishek-ireddy-946a8a222/) |
| Abhishek A M | [Profile](https://www.linkedin.com/in/mr-abhishek-988224357/) |

---

## 📜 License
**Developed for academic and research purposes.**

## ⭐ Support This Project
Give this repository a ⭐ on GitHub!

---
*Made by BMSIT CSE Students*
```
