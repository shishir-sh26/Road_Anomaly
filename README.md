# Road Hazard & Anomaly Detection System 🛣️

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![YOLOv8](https://img.shields.io/badge/YOLO-v8.3-orange?style=for-the-badge&logo=ultralytics)
![OpenCV](https://img.shields.io/badge/OpenCV-4.10-green?style=for-the-badge&logo=opencv)
![Kaggle](https://img.shields.io/badge/Kaggle-GPU_T4-blue?style=for-the-badge&logo=kaggle)

An end-to-end Computer Vision solution developed to detect road hazards, vehicle types, and pedestrians in real-time. This system is designed for dashcam integration to assist in autonomous driving safety and road infrastructure monitoring.

## 🌟 Project Overview
This project leverages the **YOLOv8 (You Only Look Once)** architecture to identify anomalies on road surfaces and surrounding traffic. By using **Transfer Learning** from the COCO dataset and fine-tuning on the **RAD (Road Anomaly Detection)** dataset, the model identifies both common traffic participants and specific road damages.

### Detected Classes:
- **Vehicles:** Cars, Motorbikes, Buses, Trucks, Vans (LMV/HMV).
- **Road Damage:** Potholes, Cracks, Manholes, Protrusions.
- **Pedestrians:** People on the road or sidewalk.
- **Infrastucture:** Speed Bumps, Road Signs, Unsurfaced Roads.

---

## 📊 Performance Metrics
The model was trained for **25 epochs** on a Tesla T4 GPU. The final validation metrics show high reliability for critical safety classes:

| Class Group | mAP@50 (Accuracy) |
| :--- | :--- |
| **LMVs (Cars/Bikes)** | **96.9%** |
| **HMVs (Buses/Trucks)** | **95.7%** |
| **Potholes** | **85.4%** |
| **Protrusions** | **76.7%** |
| **Manholes** | **64.6%** |
| **Overall Mean AP** | **78.7%** |

---

## 🛠️ Installation & Setup

### 1. Prerequisites
Ensure you have Python 3.10+ installed.
```bash
pip install ultralytics opencv-python
