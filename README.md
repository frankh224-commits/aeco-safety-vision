# AECO Safety Vision – Helmet and Vest Detection

## Project Overview

This project presents a computer vision prototype for detecting safety equipment on construction sites. The goal is to identify whether workers are wearing safety helmets and safety vests using a YOLO-based object detection model.

This type of system can support safety monitoring in AECO (Architecture, Engineering, Construction and Operations) environments by automatically screening images for compliance with safety equipment requirements.

Success Criteria:

* Detect helmets and safety vests in construction site images.
* Demonstrate inference on validation and new images.
* Provide reproducible training and inference using Google Colab.

---

## Classes

The model detects the following classes:

* Helmet
* No-Helmet
* Vest
* No-Vest

Labeling rules:

* Helmet: worker wearing a construction helmet.
* No-Helmet: worker visible without helmet.
* Vest: worker wearing a safety vest.
* No-Vest: worker visible without safety vest.

---

## Dataset

Dataset created using **Roboflow**.

Dataset details:

* Total images: **57**
* Train: **41**
* Validation: **12**
* Test: **4**
* Dataset version: **v4**

Dataset link:

https://app.roboflow.com/franciscos-workspace-df3c6/aeco_safety_demo_v1-sccci/models/aeco_safety_demo_v1-sccci/4

Dataset format: YOLO

---

## Model

Model architecture:

YOLO v11 Object Detection (Fast)

Training configuration:

* Image size: 640
* Batch size: 16
* Training environment: Roboflow + Google Colab
* Framework: Ultralytics YOLO

Training time:

* Google Colab: ~8 minutes
* Roboflow training: ~5 minutes

