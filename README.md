Real-Time Face Recognition with Streamlit

This project is a real-time face recognition application built using Streamlit, OpenCV, and the face_recognition library. The app allows users to upload a known face image and then use their webcam to recognize and label detected faces in real time.

Features

Upload a known face image for recognition

Start and stop the webcam for real-time face recognition

Detect and label known and unknown faces

Display video feed with bounding boxes around detected faces

Installation

Prerequisites

Ensure you have Python installed on your system. You also need to install the required dependencies.

Clone the Repository

git clone https://github.com/your-username/real-time-face-recognition.git
cd real-time-face-recognition

Install Dependencies

pip install streamlit opencv-python numpy face-recognition

Usage

Run the Application

streamlit run app.py

Steps to Use

Upload a known face image (JPG, JPEG, PNG format).

Click "Start Webcam" to begin real-time face recognition.

Detected faces will be labeled as "Known Person" or "Unknown Person."

Click "Stop Webcam" to stop the recognition process.

Code Explanation

The app initializes with a Streamlit interface that includes a file uploader for known face images.

The uploaded image is encoded using face_recognition to extract facial features.

When the webcam is started, frames are captured and processed in real-time.

Detected faces in the frame are compared with the known face encoding.

Bounding boxes and labels are drawn around faces based on recognition results.

Dependencies

Python 3.7+

Streamlit

OpenCV (opencv-python)

NumPy

face_recognition

Potential Issues & Fixes

Camera Not Opening: Ensure no other application is using the webcam.

No Face Found in Uploaded Image: Make sure the uploaded image contains a clearly visible face.

Multiple Faces in the Frame: The app currently recognizes only one known face at a time.

License

This project is open-source and available under the MIT License.
