# HAR PROJECT
InsightFlow
README
# InsightFlow — Human Activity Recognition Project

InsightFlow is a computer vision project focused on recognizing human activities from visual data. The system classifies 15 everyday activities, including calling, cycling, dancing, running, sleeping, and using a laptop.

At its core, InsightFlow uses a fine-tuned MobileNetV2 architecture to combine strong visual feature extraction with efficient computation. The approach incorporates preprocessing, data augmentation, performance evaluation, and Grad-CAM-based explainability to develop and understand the activity recognition model.

---

## What it does

- Classifies **15 everyday human activities** from images
- Extends the same model to **video**, sampling frames and combining predictions into a single confident answer
- Returns not just one guess but the **top 3 most likely activities**, each with a confidence score — useful when two activities look visually similar
- Runs end-to-end from raw dataset to trained model to live prediction, in one notebook

## Activities Recognized

Calling · Clapping · Cycling · Dancing · Drinking
Eating · Fighting · Hugging · Laughing · Listening to Music
Running · Sitting · Sleeping · Texting · Using Laptop

## Why this approach

- Not trained from scratch: Uses MobileNetV2 transfer learning to build on knowledge learned from large-scale image data.
- Task-specific adaptation: Fine-tunes the model to learn human activity-specific visual patterns, rather than relying only on generic image features.
- Efficiency-focused: Designed to achieve strong performance without the excessive training time and compute required by larger deep learning architectures.
- Beyond basic classification: Combines preprocessing, augmentation, fine-tuning, and explainability (Grad-CAM) into a complete pipeline.
- Application-oriented: The trained model is integrated into a practical system for image/video prediction, confidence scoring, and safety alerts.
- Lightweight but extensible: MobileNetV2 provides a computationally efficient foundation while leaving room for future improvements and additional activities.

## What we found
📊 Validation Performance

| Metric              |      Score |
| ------------------- | ---------: |
| Validation Accuracy | **93.26%** |
| Validation Loss     | **0.2853** |

## Tech Stack

TensorFlow · Keras · OpenCV · scikit-learn · Google Colab

---
