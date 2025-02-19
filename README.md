# Strawberry_OCR

## Project Description

Image Detection using StrawDi database with image tracking

### Objectives

1. **Train Object Detector**: Implement and train an object detection model on the [StrawDI dataset](https://strawdi.github.io/).
2. **Integrate Tracking Algorithm**: Incorporate the trained object detector into a tracking algorithm to perform strawberry tracking on the provided video sequence (`test.mp4`).

## Method

### Object Detection

- **Pretrained Model**: Utilize the Faster R-CNN (Region-based Convolutional Neural Network) model as a pretrained object detector for identifying strawberries in images.
- **Training**: Fine-tune the pretrained Faster R-CNN model using the StrawDI dataset to adapt it for strawberry detection.

### Tracking Algorithm

- **Tracking Approach**: Implement tracking using the Hungarian Algorithm combined with Intersection-over-Union (IoU) metrics to track detected strawberries across video frames.

## Setup and Installation

### Prerequisites

- Ability to use Google Colab

### Installation

Download the StrawDI dataset from [here](https://drive.google.com/file/d/1elFB-q9dgPbfnleA7qIrTb96Qsli8PZl/view) and change its name to dataset.zip and upload it to the colab files following instructions below (if the downloaded file is .rar, convert it to .zip with an app. DONT JUST CHANGE THE EXTENSION)

1) Import tracking.ipynb to Google Colab workspace and upload additional required files.  Example in the following picture (ignore gdrive, it will be added later through running the code)

![image](https://github.com/user-attachments/assets/41d2eccf-3bf8-4500-b144-b8b28723f0d0)

2) Run All, it should prompt you to connect your google drive account. after that it should fail somewhere, ignore.

3) Now you should have gdrive listed in the Files section, like so

![image](https://github.com/user-attachments/assets/1f97c1fe-33af-4e0e-b3da-59e29064f1d7)

4) Now ensure that in your gdrive folder, you have these folders and file uploaded. If you dont have any folders listed, create them. Follow the example image below.

![image](https://github.com/user-attachments/assets/9861974e-6673-4fa1-964d-3d41fdf95812)

5) Run All again. There are no errors that could happen that needs changing the code to fix. If there are any errors, please refer to the steps above and double check that you have done them correctly, check you file and folders hierachy. 
After fixing, go one code block above the failed one, and choose run cell and below. NEVER RUN ALL AGAIN, WILL TAKE LONG TIME TO UNZIP & TRAIN THE MODEL.

If error still persists, call me. I will go to bed now, but dont be alfraid to call me na. Im glad to help.

## Results
Detection: The object detector should be able to identify strawberries with high accuracy.
Tracking: The tracking algorithm should maintain the identity of each detected strawberry throughout the video sequence. (not 100%)
