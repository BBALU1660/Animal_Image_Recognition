


# Advanced Animal Image Recognition System

## Overview
This repository contains the implementation of an animal image recognition system developed using both YOLO v8 and YOLO v9, designed to perform with high accuracy in dynamic environments. The system demonstrates significant advancements in object detection and classification through the use of convolutional neural networks (CNNs).

## Features
- **High Accuracy**: Achieves up to 95% accuracy in detecting animals.
- **Dual YOLO Implementation**: Integrates both YOLO v8 and v9 models to optimize detection capabilities.
- **Enhanced Classification**: Utilizes CNNs to improve classification accuracy by 15%.
- **Real-Time Detection**: Optimized for real-time processing, reducing false positives by 10% and improving recognition speed by 20%.

## Setup and Installation

### Prerequisites
- Google Colab or a local setup with Anaconda.
- Python 3.9 or higher.
- Access to a GPU for training and inference is recommended.

### Installation Steps
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```

2. **Environment Setup**:
   Create and activate a Python virtual environment:
   ```bash
   conda create -n yolov_env python=3.9
   conda activate yolov_env
   ```

3. **Install Required Packages**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Dataset Preparation**:
   - Use Roboflow or Simplimg for dataset creation.
   - Ensure your dataset is structured properly for YOLO training.

5. **Modify Configuration Files**:
   - Update the paths in the `.yaml` files to point to your dataset and model weights.

### Training the Model
1. **For YOLO v8**:
   ```bash
   cd yolov8
   python train.py --img 640 --batch 16 --epochs 300 --data config_v8.yaml --weights yolov8m.pt
   ```

2. **For YOLO v9**:
   ```bash
   cd yolov9
   python train.py --img 640 --batch 16 --epochs 300 --data config_v9.yaml --weights yolov9m.pt
   ```

### Testing the Model
- Run detection on test images or video streams to evaluate model performance.
  ```bash
  python detect.py --weights path_to_weights --img 640 --conf 0.25 --source test_images/
  ```

## Results
Include example output images and performance metrics here to demonstrate the capabilities of the model in real-world scenarios.


## Contributors
- **Nikhil Balaji** - [GitHub](https://github.com/BBALU1660)
- **Srikanth** - [GitHub](https://github.com/Srikanth0903)
- **Abhinav** - [GitHub](https://github.com/AAbhinav-Chowdary)
- **Swaroop** - [GitHub](https://github.com/swaroopv4)


```

This README.md file provides a comprehensive guide for setting up, training, and testing the animal image recognition system using both YOLO v8 and YOLO v9, along with general project information. Let me know if you need any further details or adjustments!
