# Real-Time-Counting-People
📌 Project Description
This project uses OpenCV and Python to count people in real time from a video stream or webcam.
It detects people entering or leaving a defined area (e.g., doorway, shop entrance) and keeps track of the count.

By combining:

Object detection / tracking (e.g., using HOG descriptor + SVM, Haar Cascade, or a deep learning detector like MobileNet SSD / YOLO)

Counting logic (based on movement across a virtual line)

…the system can accurately count how many people pass through in each direction.

🛠 Key Features
✅ Real-time counting from webcam / CCTV feed
✅ Counts people entering & exiting separately
✅ Visual overlay: bounding boxes, IDs, and counting lines
✅ Works with multiple people at the same time
✅ Logs data (optional: save to CSV / database)

📦 Technologies Used
Python

OpenCV (for image processing & detection)

NumPy (data processing)

(Optional) Pandas (logging data)

(Optional) Deep learning frameworks (TensorFlow / PyTorch) for custom detection models

✨ How it works (Workflow)
Capture video frames from webcam or video file.

Detect people in each frame using a detector (HOG, Haar, or CNN-based).

Track detected people across frames (e.g., with centroid tracking / SORT / DeepSORT).

Draw a virtual line in the frame.

When a tracked person crosses the line, increment the counter.

Display live counts and draw bounding boxes in the video stream.

📈 Applications
Retail shops / malls for customer flow analytics

Event halls or stadiums to monitor crowd size

Smart offices or buildings to manage capacity

Public transport stations

🚀 Future Improvements
Use deep learning for better accuracy in crowded scenes

Count based on direction (entry/exit)

Deploy as a real-time web dashboard

Store historical data & generate daily / weekly reports

Integrate alerts if capacity exceeds limits
