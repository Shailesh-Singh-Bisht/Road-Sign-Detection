# Road Sign and Traffic Signal Detection System

A YOLOv8-based AI solution for detecting road signs and traffic signals in real-time. This system is designed for autonomous driving and traffic analysis applications.

## Features
- Real-time detection of road signs and traffic signals.
- Robust dataset with augmentations for diverse scenarios.
- Scalable design for integration into larger systems.

## Setup Instructions
1. Open the downloaded notebook on google collab.
2. Connect to a GPU runtime.
3. Go to file section and upload a video or image that you wan to test the model for.
4. Move the input video or file to /content/ManualTestingData folder.
5. Modify the second last code
   | weightsPath="/content/RoadSignDetection/Self-Driving-Cars-6/runs/detect/train/weights"
   !yolo task=detect mode=predict model={weightsPath}/best.pt conf=.25 source='/content/ManualTestingData/InputVideo.mp4' save=True |
   by chagning the InputVideo.mp4 to your uploaded video name.
7. Run predictions on test videos or images.
8. Download the output video by using the last code.

## Technologies Used
- Python
- YOLOv8
- Roboflow
- OpenCV
- Google Colab

## Results
Link to the tested video output : https://drive.google.com/file/d/18RE01fxlee7mfv4yS-3NhS4Zetf3BJVE/view?usp=sharing
