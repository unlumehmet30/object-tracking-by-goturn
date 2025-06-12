GOTURN-Based Object Tracking
This project implements object tracking using the GOTURN (Generic Object Tracking Using Regression Networks) algorithm. GOTURN is a deep learning-based method that tracks objects in real time by predicting their location in the next frame based on the previous one.

📸 Features
🔍 Deep learning-based object tracking using GOTURN

🎥 Real-time performance (up to 30 FPS)

🧠 Pretrained model — no online training required

🖼️ Supports video file or live webcam input

📦 Visual tracking with OpenCV

🛠️ Technologies Used
Python

OpenCV

Caffe (for GOTURN model)

NumPy

🚀 Installation
bash
Copy
Edit
# Install dependencies
pip install opencv-python numpy

# Download GOTURN model files:
# goturn.caffemodel and goturn.prototxt
You can find the pretrained model files from the original GOTURN GitHub repository: davheld/GOTURN

▶️ Usage
To run tracking on a video file:


Edit
python goturn_tracker.py --video video.mp4
To run tracking using a webcam:

Edit
python goturn_tracker.py --camera
At the start, you'll need to manually select the object to track in the first frame.

📌 Notes
The GOTURN model is pretrained — no need for retraining during tracking.

It does not support re-detection. If the object is completely lost, it will not reappear.

The algorithm is generic and works for various types of objects.

📚 References
GOTURN Paper (Held et al., 2016)

Original GOTURN GitHub Repository

OpenCV Object Tracking Guide
