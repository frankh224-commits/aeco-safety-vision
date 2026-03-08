# Error Analysis

## False Positives

Example 1
The model detected a safety vest where no vest was present.

Possible reasons:

* Similar colors or shapes confused the model.
* Limited training examples.

Example 2
Vest detected on clothing with similar color to safety vest.

Example 3
False helmet detection in complex backgrounds.

---

## False Negatives

Example 1
The model did not detect a vest even though the worker was wearing one.

Possible reasons:

* Vest partially occluded.
* Unusual angle.

Example 2
Helmet not detected in crowded scene with many workers.

Example 3
Helmet not detected in selfie-style images where objects appear larger and closer to the camera.

---

## Dataset Improvement Plan

1. Increase dataset size to at least 150+ images.
2. Add more crowded construction scenes.
3. Include different lighting conditions.
4. Add close-up helmet and vest examples.
