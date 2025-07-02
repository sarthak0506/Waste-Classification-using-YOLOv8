# Waste Detection and Management System using YOLOv8 + Streamlit
This project is an AI-powered waste classification and management system that detects waste types (e.g., plastic, metal, paper) in real-time using the YOLOv8 object detection model. The system is deployed with Streamlit, making it interactive and accessible via the browser.

# Features
Real-time object detection via:
Webcam
YouTube video stream
Uploaded video files
Uses YOLOv8 trained model (.pt) and optionally a .pkl model
Built-in tracker support (ByteTrack, BoTSORT)
Displays detection results live with confidence filtering
Simple and intuitive Streamlit UI

# Project Structure

waste-yolov8/
│
├── waste_YOLOv8.ipynb        # Jupyter notebook for model training or testing
├── helper.py                 # Main logic for video streaming, detection, and display
├── settings.py               # Configuration file for paths and options
├── weights/
│   └── yoloooo.pt            # Trained YOLOv8 model (path used in code)
├── videos/
│   ├── video_1.mp4           # Sample videos
│   └── ...
├── images/
│   ├── def.jfif              # Default image
│   └── def1.jpg
└── README.md                 # This file


# Installation
1. Clone the repository
git clone https://github.com/yourusername/waste-yolov8.git
cd waste-yolov8

3. Create and activate virtual environment (recommended)
python -m venv venv
venv\Scripts\activate       # For Windows
# source venv/bin/activate  # For Linux/Mac

3. Install dependencies
pip install -r requirements.txt

# Create requirements.txt with the following (at minimum):
streamlit
opencv-python
ultralytics
pafy
youtube-dl

# Run the Application
streamlit run helper.py
Make sure the model weights and sample videos/images are correctly placed as per the paths in settings.py.
