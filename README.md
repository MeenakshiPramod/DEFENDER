# 🐘 African Wildlife Detection using YOLO

A deep learning–based object detection system to identify African wildlife species such as **Elephant, Zebra, Rhino, and Buffalo** in images, videos, and real-time webcam feeds using the **YOLO (You Only Look Once)** framework.

This project aims to support **wildlife conservation, forest monitoring, and human–animal conflict prevention** by enabling real-time animal detection.

---

## 🚀 Features

- ✅ Real-time wildlife detection using webcam
- ✅ Trained on African Wildlife Dataset
- ✅ Supports image, video, and live camera inference
- ✅ GPU-accelerated training (CUDA)
- ✅ Model export support (ONNX, NCNN for edge devices)
- ✅ Clean and modular project structure

---

## 🦓 Detected Classes

| Class ID | Animal |
|--------|--------|
| 0 | Buffalo |
| 1 | Elephant |
| 2 | Rhino |
| 3 | Zebra |

---

## 🧠 Technologies Used

- **Python 3**
- **Ultralytics YOLO (YOLOv8 / YOLO11)**
- **PyTorch**
- **OpenCV**
- **CUDA (GPU Acceleration)**
- **Google Colab (for NCNN export)**

---

## 📂 Project Structure
```
African-Wildlife-Detection-YOLO/
│
├── african-wildlife/
│ ├── images/
│ ├── labels/
│ └── african-wildlife.yaml
│
├── webcam.py
├── export_ncnn.py
├── README.md
├── .gitignore
└── requirements.txt
```

---

## 📊 Dataset

The project uses the **African Wildlife Detection Dataset**, an object detection dataset containing annotated images of African animals captured in natural environments.

- YOLO annotation format
- Real-world conditions (occlusion, lighting variation)
- Designed for wildlife monitoring and conservation

---

## 🏋️ Model Training

To train the YOLO model:

```bash
yolo detect train model=yolo11n.pt data=african-wildlife/african-wildlife.yaml epochs=50 imgsz=640 batch=4 device=0
```

## 🌍 Applications

Wildlife conservation systems

Forest surveillance

Anti-poaching solutions

Animal intrusion detection near villages/railways

Smart camera trap automation
