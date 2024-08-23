# Bone Fracture Detection with Faster R-CNN

## Overview

This project implements a bone fracture detection system using the Faster R-CNN model. The goal is to identify and classify fractures in X-ray images to assist in medical diagnostics. The Faster R-CNN framework is employed for its high accuracy in object detection tasks.

## Technologies Used

- **Faster R-CNN**: An advanced object detection model that uses region proposal networks (RPN) and Fast R-CNN detectors to accurately locate and classify objects.
- **PyTorch**: A deep learning library used for building and training the Faster R-CNN model.
- **Torchvision**: Provides pre-trained models and tools for object detection tasks.
- **Pandas**: For managing and analyzing training results and metrics.
- **Seaborn** and **Matplotlib**: For plotting training metrics and visualizing results.
- **Roboflow**: Platform used for dataset management, annotation, and augmentations.

## Dataset

The dataset used for this project is sourced from [Roboflow](https://universe.roboflow.com/techmasters/intelligent-bone-fracture-detection-system). It consists of X-ray images annotated with bounding boxes around bone fractures. The dataset includes diverse examples of fractures to train and validate the detection model effectively.

## Results

### Training Losses

- **Mean Loss**: Average loss across all training samples.
- **Mean Loss Classifier**: Average loss from the classifier component of the model.
- **Mean Loss Box Regression**: Average loss from the box regression component of the model.
- **Mean Loss RPN Box Regression**: Average loss from the RPN box regression component.
- **Mean Loss Objectness**: Average loss for objectness prediction.

### Validation Metrics

- **Mean Average Precision (mAP)**: Measures the accuracy of fracture detection at various Intersection over Union (IoU) thresholds:
  - **mAP@50**: mAP at IoU threshold 0.50.
  - **mAP@75**: mAP at IoU threshold 0.75.
  
### for training dataset 

!['result](Bone_fracture_detection/imgs/trainInfo.png)

### for validation dataset 

!['result](Bone_fracture_detection/imgs/validInfo.png)

### Results on testDataset

!['result](Bone_fracture_detection/imgs/save.png)
## How to Clone  the Project

To clone and set up the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/bone-fracture-detection.git
   cd bone-fracture-detection
