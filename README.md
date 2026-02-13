# 🧠 YOLOv8-Based Rapunzel Character Detection System

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

- `Python 3.8+`
- `ultralytics==8.0.196`  
- `roboflow`  
- `IPython`  

Install dependencies:

```bash
pip install ultralytics==8.0.196 roboflow
```

---

## 📥 Dataset

The dataset was collected through web scraping and annotated using Roboflow with bounding box labels for Rapunzel character detection.

The dataset includes:

- Training images
- Validation images
- Test images
- Annotation files in YOLO format
- `data.yaml` configuration file

Source: https://universe.roboflow.com/davina-icasia/rapunzel

---

## 🏋️ Model Training

The YOLOv8 model was trained using the annotated Rapunzel dataset obtained from Roboflow.
During training, the model learned to detect and localize the Rapunzel character based on bounding box annotations.

The model used in this project is:
- YOLOv8 Medium (`yolov8m.pt`)

Training parameters:
- `epochs`: 25
- `imgsz` : 650
- `task` : detect

---

## 📊 Model Evaluation

After training, the model performance was evaluated using the validation and test datasets to measure detection accuracy.

Evaluation outputs include:
- Confusion matrix
- Precision, Recall, and mAP
- Training result plots

Example output files:
- `confusion_matrix.png`
- `results.png`

---

## 🔍 Prediction

After training and evaluating the model, predictions were performed on new images to test the detection capability of the trained YOLOv8 model.

Prediction result:
- Images with bounding boxes
- Saved in `runs/detect/predict/`
