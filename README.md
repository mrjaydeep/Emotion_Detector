# 😊 Emotion Detector

Real-time facial emotion detection on images and video frames, built with **TensorFlow** (deep learning) and **OpenCV** (face detection).

## How it works

1. **Face detection** — OpenCV's Haar cascade (`haarcascade_frontalface_default.xml`) locates faces in each image / frame.
2. **Emotion classification** — a TensorFlow/Keras CNN trained in `model_creation.ipynb` classifies the facial expression.
3. **GUI** — `gui.py` loads the saved model (`model_a1.json` + `model_weights1.h5`) and shows the predicted emotion.

## Project structure

```
Emotion_detection-main/
├── model_creation.ipynb               # data prep + CNN training
├── model_a1.json                      # model architecture
├── model_weights1.h5                  # trained weights
├── haarcascade_frontalface_default.xml
└── gui.py                             # desktop app for predictions
```

## Run it

```bash
pip install tensorflow opencv-python numpy pillow
cd Emotion_detection-main
python gui.py
```

## Tech

Python · TensorFlow / Keras · OpenCV · CNNs
