# Real-time Auto License Plate Recognition with Jetson Nano

This project demonstrates a real-time object detection application using NVIDIA Jetson Nano. The application leverages a pre-trained deep neural network (DNN) model to recognize and locate objects in a live camera stream. The code is written in Python and utilizes NVIDIA's Jetson Inference library for accelerated inference on the Jetson platform.

## Features
- Real-time object detection using NVIDIA's Jetson Nano.
- Supports multiple pre-trained models, including SSD-Mobilenet.
- Configurable input and output streams (e.g., camera, file, RTSP).
- Customizable detection overlays and confidence thresholds.
- Real-time FPS display and performance profiling.

## Installation

1. Clone the repository:
```
https://github.com/atharva39/Slash-Mark-Python-Advance-Task.git
```
2. Install dependencies:
Make sure you have Jetson Inference libraries installed. Follow the [Jetson Inference setup guide](https://github.com/dusty-nv/jetson-inference/tree/master) for installation.

3. You can run the script by providing the input and output URIs along with any other desired options.
```
python3 detectnet-camera.py --input_URI=camera://0 --output_URI=display://0 --network=ssd-mobilenet-v2
```

## Usage
The application supports various command-line arguments that allow you to customize the behavior of the object detection:

- input_URI: URI of the input stream (e.g., camera, video file, RTSP stream).
- output_URI: URI of the output stream (e.g., display, video file).
- --network: Specify the pre-trained model to load (e.g., ssd-mobilenet-v2).
- --overlay: Flags to customize detection overlays (e.g., box,labels,conf).
- --threshold: Minimum detection confidence threshold.
