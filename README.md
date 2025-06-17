
#Object Detection with YOLOv8

This repository contains an object detection model built using YOLOv8, specifically trained to detect the following classes:
- Car
- Bike
- Person
- Truck
- Auto

The project provides scripts and instructions to clone the repository, set up the environment, and use the trained model for detecting objects in images or videos.

---

## Features

- **YOLOv8-Based Model**: Leveraging the latest YOLOv8 architecture for fast and accurate detection.
- **Custom Trained**: Focused on five everyday classes—car, bike, person, truck, and auto.
- **Easy Inference**: Simple scripts for running detection on your own images or videos.

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Sricharan1626/objectdetction_yolov8.git
cd objectdetction_yolov8
```

### 2. Set Up the Environment

It is recommended to use Python 3.8 or higher.

Install dependencies using pip:

```bash
pip install -r requirements.txt
```

> **Note:** If `requirements.txt` is not available, make sure you have at least the following:
> - ultralytics (for YOLOv8)
> - opencv-python
> - torch

### 3. Download the Trained Model

The trained YOLOv8 model weights are provided as `my_model.pt`. If not, you can [download it from here](#) and place it in the root directory.

---

## Usage

### Detect Objects in an Image

```bash
python detect.py --weights my_model.pt --source path/to/your/image.jpg
```

### Detect Objects in a Video

```bash
python detect.py --weights my_model.pt --source path/to/your/video.mp4
```

### Arguments

- `--weights`: Path to the trained YOLOv8 weights file (use `my_model.pt`).
- `--source`: Path to the input image or video file.

The results will be saved in the `runs/detect/` directory by default.

---

## Training Graphs

All the graphs related to model training and evaluation can be found in the `my_model/train` directory.

---

## Results

- Detected objects (car, bike, person, truck, auto) will be highlighted with bounding boxes and class labels.
- Output images/videos are saved in the `runs/detect/` directory.

---

## Acknowledgements

- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)

---

For any questions or suggestions, please open an issue in this repository.

