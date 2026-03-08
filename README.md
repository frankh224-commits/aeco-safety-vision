# AECO Safety Vision

## Project Overview

This project presents a computer vision prototype for detecting safety equipment on construction sites.

The goal is to identify whether workers are wearing required safety equipment such as helmets and safety vests.

This type of system could help improve safety monitoring in AECO (Architecture, Engineering, Construction and Operations) environments.

---

## Classes

The model detects the following classes:

* Helmet
* No-Helmet
* Vest
* No-Vest

---

## Dataset

Dataset created using **Roboflow**.

Dataset details:

* Total images: 25
* Train split: 80%
* Validation split: 20%
* Test split: 0%

Dataset format: **YOLOv8**

---

## Model

Model used:

YOLOv11 Object Detection (Fast)

Training environment:

* Platform: Roboflow
* Framework: YOLO
* Image size: 640x640
* Epochs: 300 (default Roboflow training)

---

## Results

Validation metrics:

* mAP@50 ≈ 36%
* Precision ≈ 33%
* Recall ≈ 33%

Due to the small dataset size, the model performance is limited and should be considered a **prototype**.

---

## Reproducibility

To reproduce this project:

1. Open the notebook in **Google Colab**
2. Install dependencies

```
pip install ultralytics roboflow
```

3. Download dataset from Roboflow
4. Train the model
5. Run inference using the trained weights

---

## Repository Structure

```
aeco-safety-vision
│
├── README.md
├── LICENSE
│
├── docs
│   ├── class_definitions.md
│   ├── error_analysis.md
│   └── governance_checklist.md
│
├── notebooks
│
├── results
│
└── weights
```

---

## Limitations

* Small dataset (25 images)
* Limited variation in training images
* Possible false positives and false negatives

---
## Example Prediction

![Example Prediction](results/evidence/mads-eneqvist-J9jYy9S1zAk-unsplash.jpg)

## License

MIT License

