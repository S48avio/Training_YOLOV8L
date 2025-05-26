# My YOLO Project

This repository contains the YOLO object detection training and inference code.

## Project Setup

- Uses YOLOv8 for object detection.
- Dataset details in `data.yaml`.
- Training and prediction scripts included.

## Usage

```bash
# Train the model
yolo task=detect mode=train model=yolov8m.pt data=data.yaml epochs=50 imgsz=640

# Predict using the trained model
yolo task=detect mode=predict model=runs/detect/train/weights/best.pt source=images/sample.jpg conf=0.3
