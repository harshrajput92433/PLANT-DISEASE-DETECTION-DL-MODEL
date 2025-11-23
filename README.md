
# Plant Disease Detection using Deep Learning

## Overview

This project implements a deep learning–based system for automatic classification of plant leaf diseases from images. The goal is to support early diagnosis and reduce crop losses by providing an accessible tool that can identify whether a leaf is healthy or infected. The model uses image-based learning with convolutional neural networks and can be deployed on mobile or web platforms for real-time use.

## Features

* Detects multiple plant diseases and healthy conditions using leaf images
* High accuracy using transfer learning (EfficientNet, ResNet, MobileNet)
* Grad-CAM explainability for visual understanding of predictions
* Compatible with real-time camera predictions or uploaded images
* Lightweight deployment options (TFLite / ONNX / FastAPI)

## Technologies / Tools Used

Python, PyTorch/TensorFlow, EfficientNet/ResNet/MobileNet, Google Colab / Jupyter Notebook / VS Code, ONNX / TensorFlow Lite, Matplotlib, Grad-CAM visualization.

## Steps to Install & Run the Project

1. Clone the repository:

```bash
git clone https://github.com/your-username/plant-disease-detection.git
cd plant-disease-detection
```

2. Create and activate virtual environment:

```bash
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows
```

3. Install required packages:

```bash
pip install -r requirements.txt
```

4. Add dataset inside the `data/` folder (example: PlantVillage dataset)

```
data/
 ├── train/
 └── test/
```

5. Train the model:

```bash
python src/train.py --epochs 50 --batch-size 32
```

6. Run prediction:

```bash
python src/predict.py --image sample.jpg
```

## Instructions for Testing

To test with an image:

```bash
python src/predict.py --image path/to/leaf.jpg
```

To evaluate performance:

```bash
python src/evaluate.py
```

The testing output includes accuracy, precision/recall/F1-score, confusion matrix, and Grad-CAM heatmaps.

---

If you want, I can now provide the **PowerPoint PPT**, **project abstract**, or **final report**. Which one should I generate next?
