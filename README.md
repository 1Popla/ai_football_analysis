## Project Documentation
# !IMPORTANT!
To run and analyze, download the model and video input from the link below

https://drive.google.com/drive/folders/1zyPnplAeBdt93AI6zkutVYxU5_SCP7Yj?usp=drive_link

- "last.pt" place in models directory
- "08fd33_4.mp4" place in input_videos directory

# Overview

- This project implements a video processing pipeline to analyze and extract insights from sports videos. 
- It includes functionalities for object detection, tracking, and various analyses such as team assignment, ball tracking, and speed estimation.

# Usage
- Processing a Video:
- Place the video file you want to process in the input_videos directory.
- Modify the main script main.py to specify the desired input video and output paths.
- Run the script

# Processing
- The main processing steps include:
- Object Detection: Detects players and ball using YOLO.
- Tracking: Tracks objects across frames.
- Camera Movement Estimation: Estimates camera movement and adjusts track positions accordingly.
- Team Assignment: Assigns team colors to players based on visual cues.
- Ball Tracking: Interpolates ball positions and assigns the ball to a specific player.
- Speed and Distance Estimation: Estimates the speed and distance of tracked objects.
- Customization:Various aspects of the processing pipeline can be customized:
- Models: The object detection model can be swapped out for a different one by modifying models/last.pt.
- Stubs: Preprocessed data can be reused via stub files in the stubs directory.
- Drawing Annotations: Adjustments to how annotations are drawn can be made in the draw_annotations method.
