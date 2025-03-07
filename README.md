# Enhancing-Deep-Learning-Paradigms-for-Fire-and-Smoke-detection
# Fire and Smoke Detection using Deep Learning (YOLOv11)

This project implements fire and smoke detection using "YOLOv11", an online dataset from "Roboflow", and real-time notifications via "Twilio". The system can detect fire and smoke from images and videos, sending alerts when a fire hazard is detected.

 1.Features
- Fire & Smoke Detection**: Uses "YOLOv11" for real-time detection.
- Dataset: Extracted from "Roboflow" for training.
- Twilio Notifications: Sends SMS alerts upon detection.
- Fast and Efficient: Optimized deep learning model for accurate detection.

2.Dataset
- The dataset was obtained from [Roboflow](https://roboflow.com).
- It consists of labeled images containing "fire and smoke scenarios".
- Data augmentation was applied to improve model generalization.

3.Installation & Setup
Clone the Repository:

[git clone](https://github.com/KOTA-HARSHITHA/Enhancing-Deep-Learning-Paradigms-for-Fire-and-Smoke-detection.git)
cd Enhancing-Deep-Learning-Paradigms-for-Fire-and-Smoke-detection.

4.Install Dependencies 
- [Installation](pip install -r requirements.txt)

5.Download the dataset from Roboflow.

6.Run the Detection
- python detect.py --source input_video.mp4 --weights best.pt

# Model Training
- Preprocess the dataset using the YOLOv11 format.
- Train the model with:(python train.py --data dataset.yaml --epochs 50 --weights yolov11.pt)
- Evaluate performance on test data.

## Twilio SMS Alerts
- Set up Twilio: Create an account at Twilio.
- Configure API keys in config.py
- Enable alerts in your script:python alert_system.py






  











