# DL_Project
# Person Tracking Project

## Overview
This project utilizes facial recognition techniques to identify and track individuals across multiple video streams. The system is built using PyTorch and leverages pre-trained models for face detection and recognition.

## Key Features
- Face detection using FastMTCNN (Multi-task Cascaded Convolutional Networks)
- Face recognition using a fine-tuned InceptionResnetV1 model
- Real-time tracking across multiple video streams
- Data augmentation for improved model performance
- Support for both image and video processing

## Prerequisites
- Python 3.x
- PyTorch
- OpenCV
- facenet-pytorch
- NumPy

## Project Structure
The project consists of several key components:

1. **Data Preparation**: 
   - The system uses a dataset of facial images organized in directories by person.
   - Data augmentation techniques are applied to enhance the training dataset.

2. **Model Training**:
   - An InceptionResnetV1 model is fine-tuned on the prepared dataset.
   - The training process includes both training and validation phases.

3. **Face Detection and Recognition**:
   - FastMTCNN is used for face detection in images and video frames.
   - The trained InceptionResnetV1 model is used for face recognition.

4. **Video Processing**:
   - The system can process multiple video streams.
   - Detected faces are tracked and labeled in real-time.

5. **Output Generation**:
   - Processed frames are compiled into an output video with labeled faces.

## Usage
1. Prepare your dataset in a directory structure where each subdirectory represents a person and contains their images.
2. Run the training script to fine-tune the InceptionResnetV1 model on your dataset.
3. Use the trained model to process images or videos for face detection and recognition.

## Key Functions
- `collate_fn`: Custom function for data loading
- `create_video_from_frames`: Generates output video from processed frames

## Model Details
- Face Detection: FastMTCNN
- Face Recognition: Fine-tuned InceptionResnetV1
- Training: Uses CrossEntropyLoss and Adam optimizer

## Output Video
https://drive.google.com/file/d/1TtfFJIqW03E5JM2v8KxJ0txt6Pc0oAeB/view?usp=drive_link
