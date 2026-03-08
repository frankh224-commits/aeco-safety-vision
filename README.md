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
* Train: **32**
* Validation: **19**
* Test: **6**
* Dataset version: **v5**

Dataset link:

https://app.roboflow.com/franciscos-workspace-df3c6/aeco_safety_demo_v1-sccci/models/aeco_safety_demo_v1-sccci/5

Dataset format: YOLO

---

## How to Reproduce (Google Colab)

This project can be reproduced entirely in the cloud using Google Colab.

Steps:

1. Open the training notebook from this repository in Google Colab.

2. Install dependencies:

pip install ultralytics roboflow

3. Load the dataset from Roboflow.

4. Train the YOLO model using the training notebook.

5. The notebook will automatically generate:

* training metrics
* validation results
* prediction outputs

6. Run the inference notebook to test the trained model on new images.

Expected runtime:

* Google Colab CPU: ~8 minutes
* Roboflow training: ~5 minutes


## Results Summary

Model performance on the validation dataset:

* Precision: 38.1%
* Recall: 34.9%
* mAP@50: 37.3%
* mAP50-95: 26.98%

### Key Conclusions

1. The model demonstrates moderate precision, meaning it can correctly identify safety equipment when detected.

2. Recall is relatively low, indicating the model still misses several helmets and safety vests.

3. Detection performance decreases in complex scenarios such as crowded scenes, small helmets, strong lighting, or selfie-style images.

These results indicate that increasing the dataset size and diversity would significantly improve model performance.



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
* Roboflow training: ~9 minutes

