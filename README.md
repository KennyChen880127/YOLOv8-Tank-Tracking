


# YOLOv8-Tank-Tracking
In the modern battlefield environment, tank identification and tracking are of paramount importance for strategic intelligence and operational efficiency. Our laboratory is dedicated to developing advanced automatic tank identification and tracking technology, utilizing YOLOv8 object detection for tank recognition. However, due to the presence of both friendly and enemy tanks on the battlefield, this experiment incorporates the [tracking](https://docs.ultralytics.com/modes/track/) functionality of YOLOv8, combined with a user-friendly interface design. This allows for the continuous tracking of enemy tanks by specifying their IDs using a mouse.) functionality of YOLOv8, combined with a user-friendly interface design. This allows for the continuous tracking of enemy tanks by specifying their IDs using a mouse.

P.S.: You can also use [COCO dataset](https://cocodataset.org/#home) or train on your prepared dataset for ID tracking.

## YOLOv8
[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and easy to use, making it an excellent choice for a wide range of object detection and tracking, instance segmentation, image classification and pose estimation tasks.

## Features
* Multiple instances of the same class can appear on the screen simultaneously. You can click on the canvas with the mouse to select one to track and return its coordinates.
* Design a simple user interface with the following functions: screenshot, record video, start/stop recognition, start/stop tracking.

## Steps to run Code
### Create Virtual Environment
* Pip install the ultralytics package including all [requirements](<https://github.com/ultralytics/ultralytics/blob/main/requirements.txt>) in a [Python>=3.8](https://www.python.org/) environment with [PyTorch>=1.8](https://pytorch.org/get-started/previous-versions/).

        pip install -r requirements.txt
* For alternative installation methods including [Conda](https://anaconda.org/conda-forge/ultralytics), [Docker](https://hub.docker.com/r/ultralytics/ultralytics), and Git, please refer to the [Quickstart Guide](https://docs.ultralytics.com/quickstart/).

        pip install ultralytics
* Clone the repository
  
        git clone https://github.com/KennyChen880127/YOLOv8-Tank-Tracking.git
* Goto cloned folder
  
        cd YOLOv8-Tank-Tracking
### Predicting
You can use the tank dataset I've already trained with YOLOv8n for predictions, or you can use the models provided by YOLOv8, see [Detection Docs](https://docs.ultralytics.com/tasks/detect/) for usage examples with these models.

* [Tank](https://drive.google.com/file/d/1JiVR8DMc9CoGRUi7SnDLNyOuPOFNdB4X/view?usp=drive_link)
* [YOLOv8n](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt)
* [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt)
* [YOLOv8m](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt)
* [YOLOv8l](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8l.pt)
* [YOLOv8x](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8x.pt)

* Use the following command to trace

        python tank_tracking.py --weights weights/tank.pt --source example_video/example_tank.mp4
### HMI Operation
The button `Capture Image` captures the current screen and saves it to `Image Result`. `Start Recording` is for recording videos, and the recorded video is saved in `Video Result`. `Start Detecting` begins object recognition, while `Start Tracking` activates tracking mode. You can start tracking by clicking anywhere inside one of the bounding boxes on the screen. `Exit Program` is used to close the program.
  
### Results
| Tank Experiment Results | Person Experiment Results |
| ------------- | ------------- |
| ![tank_tracking](https://github.com/KennyChen880127/YOLOv8-Tank-Tracking/assets/99500847/084e3b85-3a5f-4a3a-b92d-584c6a4912f2) | ![person_tracking](https://github.com/KennyChen880127/YOLOv8-Tank-Tracking/assets/99500847/c2ee43c3-1695-47c1-bba6-c89f64b0dae3) |
