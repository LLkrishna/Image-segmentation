# Custom YOLOv5 Eyewear Detection

## Overview

This project focuses on detecting eyewear (glasses/spectacles) in images using a custom-trained YOLOv5 model. The dataset was curated using Roboflow, which facilitated the annotation and splitting of the dataset. The project integrates YOLOv5 for object detection and the Segment Anything Model (SAM) for advanced image segmentation.

## Technologies Used

- YOLOv5: Train a custom YOLOv5 model on the dataset.
- PyTorch: Deep learning framework for implementing and training the YOLOv5 model and Implement the Segment Anything Model for segmentation tasks.
- Roboflow: Manage and preprocess dataset using Roboflow, annotated images of spectacles.
- Segment Anything Model (SAM): Use Segment Anything Model (SAM) for advanced segmentation.

## Models Used

- YOLOv5: A state-of-the-art object detection model used to train on a custom dataset of eyewear.
- Segment Anything Model (SAM): Used for segmenting detected eyewear from the images.

## Process Followed

1. **Clone YOLOv5 Repository:** Obtained the YOLOv5 codebase from GitHub.
2. **Install Dependencies:** Installed all required dependencies for running YOLOv5.
3. **Dataset Preparation:** Used Roboflow to download and prepare a custom dataset of annotated eyewear images.
4. **Model Configuration:** Created a custom YOLOv5 configuration file tailored to the eyewear dataset.
5. **Training:** Trained the YOLOv5 model on the prepared dataset for 200 epochs.
6. **Inference:** Performed inference on test images to detect eyewear.
7. **Segmentation:** Used SAM to segment the detected eyewear from the images for better visualization.

## Dataset

- The dataset includes 128 images of spectacles, annotated with bounding boxes indicating the presence and location of eyewear.
- Annotations are in YOLO format, and the dataset is split into training, testing, and validation sets.

## Outputs

- **Detection Results:** Images with detected eyewear and corresponding bounding boxes.
- **Segmentation Results:** Segmented eyewear from the images using SAM, visualized against a plain white background.

## Acknowledgements

Special thanks to Roboflow for providing tools and infrastructure to manage and annotate the dataset efficiently. More information on Roboflow can be found at [roboflow.com](https://roboflow.com/).

## License

This project is licensed under the MIT License.
