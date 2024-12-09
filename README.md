# AI-Enabled Weapon Detection System

This project leverages the YOLOv5 deep learning model to detect weapons in images and videos. The system includes training, prediction, and text-to-speech functionality for enhanced usability and safety.

---

## Project Structure

```plaintext
AIYolov5/
│
├── content/yolov5/runs/train/yolov5s_results/
│   ├── best.pt        # Trained weights for the best model
│   ├── last.pt        # Trained weights from the last epoch
│   ├── result_image   # Sample detection results image
│
├── PredictionCode/
│   ├── prediction.py  # Code for predicting weapons in images/videos
│   ├── text_to_speech.py # Converts detection results into spoken alerts
│   └── requirements.txt # Dependencies for running the project
│
├── TrainingCode/
│   ├── data.yaml      # Contains class names for the dataset (e.g., "weapon")
│   ├── train.py       # Code for loading dataset and training the model
│   └── roboflow_api.py # Code for loading the dataset from Roboflow API
