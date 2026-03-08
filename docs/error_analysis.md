# Error Analysis

## False Positive Example

Image: example_fp.jpg

Observation:
The model detected a helmet where there was no helmet.

Possible reasons:
- The model confused similar shapes.
- The dataset is very small (25 images).
- Limited variation in training images.

---

## False Negative Example

Image: mitchell-luo-TtX79Vkm8gs-unsplash.jpg

Observation:
The worker is wearing a helmet, but the model did not detect it.

Possible reasons:
- The dataset used for training is small.
- The helmet angle differs from training images.
- Lighting conditions are different from the training set.

---

## Dataset Improvements

1. Increase dataset size to at least 100+ images.
2. Include different angles of helmets and vests.
3. Add more construction environments.
