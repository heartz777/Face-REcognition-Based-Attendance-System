# Face-REcognition-Based-Attendance-System
An automated computer vision application designed to streamline attendance collection using real-time face detection and 128-dimensional facial embedding comparisons[cite: 1]. Built using Python, OpenCV, and the `face_recognition` library.

## Features
* **Automated Face Encoding:** Automatically parses reference photos from the image directory and extracts 128-d vector embeddings using deep metric learning.
* **Optimized Real-Time Processing:** Reduces processing frame resolution to 25% scale to maintain smooth video processing.
* **Duplicate Prevention Cooldown:** Enforces a configurable 600-second (10-minute) cooldown per user to eliminate duplicate logs.
* **Visual Frame Feedback:** Displays color-coded bounding boxes on live camera feeds (Green = Recognized, Red = Unknown).
* **Daily Log Generation:** Automatically creates and appends attendance records into formatted `.csv` files (`YYYY-MM-DD_Attendance.csv`).

## Tech Stack
* **Language:** Python 3.x
* **Computer Vision:** OpenCV (`cv2`)
* **Facial Recognition:** `face_recognition` (dlib wrapper)
* **Numerical Operations:** `numpy`
* **Data Serialization & Logging:** `pickle`, `csv`
