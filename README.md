## 🌲🔥 Forest Fire & Smoke Detection (YOLOv11s)

A **real-time forest fire & smoke detection system** powered by **YOLOv11s**, trained on a **custom dataset of 6,500+ labeled images**.
This project focuses on **early fire detection** to help prevent devastating wildfires through rapid alerts.

---

## 📌 Features

* **🔥 Detects both Fire and Smoke** with high accuracy.
* **📷 Supports multiple video sources** — webcam, CCTV (RTSP), and video files.
* **🖥️ Lightweight & Fast** — optimized with YOLOv11s for deployment on laptops, edge devices, and Raspberry Pi.
* **📊 Well-trained & tested** on a large, diverse dataset.
* **⚡ Low latency** — capable of running in near real-time.

---

## 📊 Model Performance

| Metric               | Value  |
| -------------------- | ------ |
| **Precision**        | 82.41% |
| **Recall**           | 78.12% |
| **mAP\@50**          | 85.05% |

*(Performance measured on validation dataset; results may vary based on hardware.)*

---

## 🗂 Dataset

* **Classes:**
![labels](https://github.com/user-attachments/assets/d3c21d71-dfe2-42e4-be72-2dc00047da31)

  1. Fire
  2. Smoke
  3. Other/Background
* **Size:** 6,500+ images
* **Annotations:** YOLO format
* **Sources:** Combination of open-source datasets + manually curated and cleaned web-scraped images.

---

## ⚙️ Installation

1️⃣ Clone the repo

```bash
git clone https://github.com/yourusername/forest-fire-detection.git
cd forest-fire-detection
```

2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

▶️ Usage
1. Run with Webcam
Open the notebook and run all cells:

```bash
jupyter notebook Forest_Fire_Detection.ipynb
```
Make sure the source in the notebook is set to 0 for webcam input.

3. Run with CCTV Stream
In the notebook, set:
```bash
weights = "best.pt"
source = "rtsp://username:password@ip:port/stream"
```
Then run the inference cell.

3. Run on Raspberry Pi
Use YOLOv11s for faster inference.

Install lightweight dependencies and use hardware-accelerated OpenCV (libopencv-dev and opencv-python-headless).

Consider lowering the resolution for real-time detection.

---

## 📦 Deployment Scenarios

* **Forest Lookout Towers** → monitor live CCTV feeds.
* **Drones** → detect fires from aerial footage.
* **IoT Devices** → automated early warning systems.

---
