# About Roboflow

Roboflow is a comprehensive platform designed to simplify and enhance the development of computer vision applications. It offers tools for every stage of the computer vision pipeline, including data collection, organization, annotation, preprocessing, model training, and deployment. Roboflow is widely used by developers, researchers, and enterprises to build robust computer vision models without requiring deep expertise in machine learning.

## Key Features of Roboflow

- **Data Management:** Supports various data formats and integrates with cloud storage solutions like AWS S3 and Google Cloud. It offers tools for organizing and annotating visual data, including automated labeling with models like Segment Anything (SAM).
- **Model Training and Deployment:** Supports popular frameworks such as TensorFlow, PyTorch, and YOLO. Users can train custom models and deploy them using the Roboflow API or on edge devices like NVIDIA Jetson and Raspberry Pi.

# Custom YOLOv5 Dataset for Eyewear Detection

This repository contains a custom dataset for training a YOLOv5 model to detect eyewear (glasses/spectacles). The dataset includes annotated images, split into training, testing, and validation sets, and is ready to be used for model training.

## Dataset Overview

The dataset consists of 128 images of spectacles, each annotated with bounding boxes to indicate the presence and location of the eyewear. The annotations were created using Roboflow, which also managed the dataset splitting and provided the necessary configuration files.

## Directory Structure

The dataset is organized into the following structure:

dataset/
│
├── train/
│ ├── images/
│ └── labels/
│
├── test/
│ ├── images/
│ └── labels/
│
├── val/
│ ├── images/
│ └── labels/
│
├── data.yaml
└── README.md


- **train/, test/, val/:** Directories containing images and corresponding label files for training, testing, and validation respectively.
- **data.yaml:** Configuration file with dataset paths and class names.
- **README.md:** This readme file.

## Annotations

Annotations are provided in YOLO format. Each image has a corresponding text file in the labels/ directory, containing the bounding box coordinates and class labels.

## Data Preparation

The dataset was prepared using Roboflow's API, which facilitated the following steps:

- **Annotation:** Created bounding boxes for each image.
- **Dataset Split:** Automatically split the dataset into training, testing, and validation sets.
- **Configuration Files:** Generated data.yaml and README.md files.

## Dataset Usage

Download the dataset directly from the Roboflow dashboard or use the provided API endpoint to fetch the dataset programmatically through the Roboflow API. Follow the instructions provided in the data.yaml file for correct paths and usage.

You can find my dataset through this [link](https://app.roboflow.com/image-segmentation-lfxjl/specs-vzzww/1).

## Acknowledgements

Special thanks to Roboflow for providing tools and infrastructure to manage and annotate the dataset efficiently. More information on Roboflow.
Provided by a Roboflow user
License: CC BY 4.0