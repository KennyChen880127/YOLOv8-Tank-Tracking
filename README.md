


# YOLOv8 Tank Tracking
In the modern battlefield environment, tank identification and tracking are of paramount importance for strategic intelligence and operational efficiency. Our laboratory is dedicated to developing advanced automatic tank identification and tracking technology, utilizing YOLOv8 object detection for tank recognition. However, due to the presence of both friendly and enemy tanks on the battlefield, this experiment incorporates the [tracking](https://docs.ultralytics.com/modes/track/) functionality of YOLOv8, combined with a user-friendly interface design. This allows for the continuous tracking of enemy tanks by specifying their IDs using a mouse.) functionality of YOLOv8, combined with a user-friendly interface design. This allows for the continuous tracking of enemy tanks by specifying their IDs using a mouse.

P.S.: You can also use [COCO dataset](https://cocodataset.org/#home) or train on your prepared dataset for ID tracking.

## YOLOv8
[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making it an excellent choice for a wide range of object detection and tracking, instance segmentation, image classification and pose estimation tasks.

## Features
* Multiple instances of the same class can appear on the screen simultaneously. You can click on the canvas with the mouse to select one to track and return its coordinates.
* Design a simple user interface with the following functions: screenshot, record video, start/stop recognition, start/stop tracking.

### HMI Operation
The button `Capture Image` captures the current screen and saves it to `Image Result`. `Start Recording` is for recording videos, and the recorded video is saved in `Video Result`. `Start Detecting` begins object recognition, while `Start Tracking` activates tracking mode. You can start tracking by clicking anywhere inside one of the bounding boxes on the screen. `Exit Program` is used to close the program.
  
### Results
| Tank Experiment Results | Person Experiment Results |
| ------------- | ------------- |
| ![tank_tracking](https://github.com/KennyChen880127/YOLOv8-Tank-Tracking/assets/99500847/50a67e71-02c3-4aac-927b-54815b7da0a2) | ![person_tracking](https://github.com/KennyChen880127/YOLOv8-Tank-Tracking/assets/99500847/b3dce3f5-f321-42be-8d26-a7fd24068551) |
