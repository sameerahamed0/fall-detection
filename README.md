# 🚨 YOLO-MINESAFE — Real-Time Fall Detection System

> **AI-powered real-time worker fall detection and safety monitoring system using YOLOv8 and computer vision.**

YOLO-MINESAFE is an AI-based workplace safety system designed to detect **worker falls in real time** using surveillance cameras. The system uses **YOLOv8 object detection** and computer vision techniques to identify dangerous incidents and generate alerts, helping improve worker safety in environments such as construction sites, mining areas, warehouses, and industrial workplaces.

---

## 🎯 Project Overview

Workplace falls are one of the major safety hazards in industrial environments. Traditional surveillance systems require continuous human monitoring, which can be inefficient and prone to missed incidents.

YOLO-MINESAFE automates this process by continuously analyzing video streams and detecting workers who may have fallen.

### 🔥 Key Features

* 🎥 Real-time video surveillance
* 🤖 YOLOv8-based object detection
* 🧍 Worker detection
* 🚨 Fall detection
* 📹 Support for live camera/video input
* ⚡ Real-time inference
* 🔔 Automated alert generation
* 📊 Detection confidence monitoring
* 🖥️ User-friendly monitoring interface
* 🏭 Designed for industrial safety applications

---

## 🧠 How It Works

```text
Camera / Video Input
        ↓
   Video Processing
        ↓
      YOLOv8
        ↓
   Object Detection
        ↓
   Fall Detection
        ↓
  Confidence Analysis
        ↓
   🚨 Alert System
```

The system processes video frames continuously and uses the trained YOLOv8 model to identify workers and potential fall incidents.

---

## 🛠️ Tech Stack

| Technology      | Purpose                           |
| --------------- | --------------------------------- |
| 🐍 Python       | Core programming language         |
| 🤖 YOLOv8       | Object detection & fall detection |
| 👁️ OpenCV      | Image/video processing            |
| 🔥 PyTorch      | Deep learning framework           |
| 📊 NumPy        | Numerical processing              |
| 🌐 Streamlit    | Web-based monitoring interface    |
| 🐙 Git & GitHub | Version control                   |

---

## 📁 Project Structure

```text
YOLO-MINESAFE/
│
├── dataset/
│   ├── images/
│   ├── labels/
│   └── data.yaml
│
├── models/
│   └── best.pt
│
├── runs/
│   └── detect/
│
├── app.py
├── detect.py
├── train.py
├── requirements.txt
├── README.md
└── .gitignore
```

> Project structure may vary depending on the implementation and training workflow.

---

## ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/sameerahamed0/YOUR-REPOSITORY-NAME.git
```

### 2️⃣ Navigate to the project

```bash
cd YOUR-REPOSITORY-NAME
```

### 3️⃣ Create a virtual environment

```bash
python -m venv venv
```

### 4️⃣ Activate the environment

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

### 5️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 Running the Project

### Run the detection system

```bash
python detect.py
```

### Run the Streamlit application

```bash
streamlit run app.py
```

The application will open in your browser and allow you to monitor the video stream and detected incidents.

---

## 🧠 Model Training

The model was trained using **YOLOv8** on a custom dataset containing workplace/person fall scenarios.

Example training command:

```bash
yolo detect train \
    data=data.yaml \
    model=yolov8n.pt \
    epochs=100 \
    imgsz=640
```

### Training Pipeline

```text
Dataset Collection
       ↓
Data Annotation
       ↓
Dataset Preprocessing
       ↓
YOLOv8 Training
       ↓
Model Validation
       ↓
Performance Evaluation
       ↓
Real-Time Deployment
```

---

## 📊 Model Evaluation

The trained model can be evaluated using common object detection metrics:

* Precision
* Recall
* mAP@50
* mAP@50-95
* Inference Speed
* FPS

Example:

```text
Precision  : XX.XX%
Recall     : XX.XX%
mAP@50     : XX.XX%
mAP@50-95  : XX.XX%
FPS        : XX
```

> Replace the placeholder values with your actual training results.

---

## 🚨 Fall Detection Workflow

When a person is detected as falling:

```text
Person Detected
      ↓
Fall Detected
      ↓
Confidence Check
      ↓
Incident Confirmed
      ↓
🚨 Alert Generated
```

This enables faster identification of potentially dangerous situations and can reduce dependence on continuous manual monitoring.

---

## 🖥️ Application

The monitoring interface provides:

* Live video feed
* Detected objects
* Detection confidence
* Fall status
* Real-time alerts
* Monitoring information

### 📸 Screenshots

Add your project screenshots here:

```markdown
<img width="1813" height="1079" alt="Screenshot 2026-02-26 104248" src="https://github.com/user-attachments/assets/a6a87a29-f77c-489c-b572-c3969c5a8f33" />
<img width="1919" height="1079" alt="Screenshot 2026-02-26 104335" src="https://github.com/user-attachments/assets/d137ebdd-057d-44e2-8be0-3d9c76da4661" />
<img width="1906" height="1058" alt="Screenshot 2026-02-26 104409" src="https://github.com/user-attachments/assets/ec0d2cab-5de5-4b94-8b5a-4542cd7fe0a9" />
<img width="1907" height="1061" alt="Screenshot 2026-02-26 104513" src="https://github.com/user-attachments/assets/541d179d-a1d6-4941-ba09-4fd84e15a759" />
<img width="1904" height="1071" alt="Screenshot 2026-02-26 104607" src="https://github.com/user-attachments/assets/d45fabe7-429e-4b93-bfeb-8556a23e57d8" />
<img width="1451" height="961" alt="Screenshot 2026-05-07 233418" src="https://github.com/user-attachments/assets/aeea47d7-98be-4a9f-bfc7-9f2306505286" />
<img width="959" height="461" alt="Screenshot 2026-04-17 142024" src="https://github.com/user-attachments/assets/38ee939e-774a-45ce-9cdb-44c6e9970707" />

```

---

## 🎯 Applications

YOLO-MINESAFE can be adapted for:

* 🏗️ Construction sites
* ⛏️ Mining environments
* 🏭 Manufacturing facilities
* 📦 Warehouses
* 🏢 Industrial workplaces
* 👷 Worker safety monitoring
* 🏥 Assisted living environments

---

## 🔮 Future Improvements

* [ ] SMS / Email alerts
* [ ] WhatsApp / Telegram notifications
* [ ] Multiple camera support
* [ ] Cloud-based monitoring
* [ ] Edge-device deployment
* [ ] CCTV integration
* [ ] Incident history and analytics
* [ ] Automatic incident screenshots
* [ ] GPS/location-based incident tracking
* [ ] Mobile application
* [ ] Docker deployment
* [ ] Advanced pose estimation
* [ ] Integration with IoT safety systems

---

## 📈 Project Impact

YOLO-MINESAFE demonstrates how **computer vision and deep learning can be applied to real-world industrial safety problems**.

The system aims to:

> **Detect → Analyze → Alert → Respond**

By automating fall detection, organizations can potentially improve incident response times and enhance workplace safety monitoring.

---

## 👨‍💻 Developer

### Sameer Ahamed

**B.Tech(Hons) — Artificial Intelligence & Data Science**

I'm interested in building real-world solutions using:

```text
Artificial Intelligence
Machine Learning
Computer Vision
Data Engineering
Generative AI
Cloud Computing
```

### 🌐 Connect With Me

🐙 GitHub:
https://github.com/sameerahamed0

💼 LinkedIn:
www.linkedin.com/in/sameer-ahamed-s-405485278

📧 Email:
sameeahamed1@gmail.com

---

## ⭐ Support

If you find this project useful or interesting, consider giving the repository a ⭐ on GitHub!

---

## 📜 License

This project is intended for educational and research purposes.
paper published in IJSART as Researcher Paper ID:IJSARTV124104890
LINK:https://ijsart.com/yolo-minesafe-a-vision-based-abnormal-fall-detection-and-emergency-alert-framework-for-isolated-mining-workers-104890

---

# 🚀 YOLO-MINESAFE

**Real-Time AI-Powered Fall Detection for Safer Workplaces.**

> *"Detect early. Alert instantly. Protect workers."*
