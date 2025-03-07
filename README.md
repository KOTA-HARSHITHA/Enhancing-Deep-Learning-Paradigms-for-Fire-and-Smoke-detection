
Fire and Smoke Detection using Deep Learning (YOLOv11)

This project implements fire and smoke detection using "YOLOv11", an online dataset from "Roboflow", and real-time notifications via "Twilio". The system can detect fire and smoke from images and videos, sending alerts when a fire hazard is detected.

Features
- Fire & Smoke Detection: Uses YOLOv11 for real-time detection.
- Dataset**: Extracted from Roboflow for training.
- Twilio Notifications: Sends SMS alerts upon detection.
- Fast and Efficient: Optimized deep learning model for accurate detection.

Dataset
- The dataset was obtained from [Roboflow](https://roboflow.com/).
- It consists of labeled images containing fire and smoke scenarios.
- Data augmentation was applied to improve model generalization.

Installation & Setup
1. Clone the Repository**
```bash
git clone https://github.com/KOTA-HARSHITHA/Enhancing-Deep-Learning-Paradigms-for-Fire-and-Smoke-detection.git
cd fire-smoke-detection
```

2. Download the Dataset
- Visit [Roboflow](https://roboflow.com/), download the dataset, and place it in the `dataset/` directory.

3 Run the Detection
```bash
python detect.py --source input_video.mp4 --weights best.pt
```

 Model Training
1. Preprocess the dataset** using the YOLOv11 format.
2. Train the model with:
   ```bash
   python train.py --data dataset.yaml --epochs 50 --weights yolov11.pt
   ```
3. Evaluate performance on test data.

Twilio SMS Alerts

1. Set up Twilio**: Create an account at [Twilio](https://www.twilio.com/).
2. Configure API keys** in `config.py`:
   ```python
   TWILIO_ACCOUNT_SID = "your_account_sid"
   TWILIO_AUTH_TOKEN = "your_auth_token"
   TWILIO_PHONE_NUMBER = "your_twilio_number"
   RECEIVER_PHONE_NUMBER = "your_phone_number"
   ```
3. Enable alerts in your script**:
   ```bash
   python alert_system.py
   ```
Results and Output:
1.The Fire and Smoke is detected with boundary box and it's percentage.
2.The Alert! notification is sent to the user.

