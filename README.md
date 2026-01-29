# 🧠 Implementation of YOLOv8 for Image Detection of Rapunzel Character

This project implements **YOLOv8 (You Only Look Once version 8)** for detecting the **Rapunzel character** in images.  
The system is built using the **Ultralytics YOLOv8 framework** and a dataset obtained from **Roboflow**.

The workflow includes dataset downloading, model training, evaluation, and prediction.

---

## 🚀 Features

- Automatic dataset download from Roboflow  
- Training YOLOv8 model for character detection  
- Model evaluation with performance metrics  
- Image prediction and visualization  
- End-to-end object detection pipeline  

---

## 📦 Requirements

- Python 3.8+
- ultralytics==8.0.196  
- roboflow  
- IPython  

Install dependencies:

```bash
pip install ultralytics==8.0.196 roboflow
```

## 📥 Dataset

The dataset is provided by Roboflow and contains images of the Rapunzel character with bounding box annotations.
The dataset includes:

- Training images
- Validation images
- Test images
- Annotation files in YOLO format
- `data.yaml` configuration file

## 🏋️ Model Training

The dataset is provided by Roboflow and contains images of the Rapunzel character with bounding box annotations.

The model used in this project is:
- YOLOv8 Medium (`yolov8m.pt`)

Training parameters:
- `epochs`: 25
- `imgsz` : 650
- `task` : detect

## 📊 Model Evaluation

The dataset is provided by Roboflow and contains images of the Rapunzel character with bounding box annotations.
The dataset includes:

Evaluation outputs include:
- Confusion matrix
- Precision, Recall, and mAP
- Training result plots

Example output files:
- `confusion_matrix.png`
- `results.png`

## 🔍 Prediction

Prediction result:
- Images with bounding boxes
- Saved in `runs/detect/predict/`
