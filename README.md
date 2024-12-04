Face Detection-Based Attendance System
This project implements a real-time facial recognition-based attendance system using Python and OpenCV. It detects faces from a live webcam feed, recognizes them against a predefined dataset, and logs the attendance of recognized individuals into a file.

Features:
Real-Time Detection and Recognition:
Detects faces in a video stream.
Recognizes known faces using a custom face encoding system.
Automated Attendance Logging:
Records recognized names into an attendance log file.
Custom Dataset:
Allows users to create a dataset of known individuals by storing their images in a specified folder.

File Overview
1. Face Detection Based Attendance System.py
This is the main script that:

Captures a live video stream using the webcam.
Utilizes the Face class from face_encoding.py for facial recognition.
Displays a live video feed with bounding boxes and names around recognized faces.
Logs recognized individuals into attendance_log.txt.
Key functionalities:

Live Detection and Display: Detected faces are highlighted with red rectangles, and names are displayed above the faces.
Attendance Logging: Unique names are written to a log file.
2. attendance_log.txt
This text file stores the names of recognized individuals. Each name is logged only once during a session. Example content:

Copy code
student_1
student_2
3. Example Output (Image Preview)

The system detects a face and labels it (e.g., "student_1").
Red rectangles highlight the detected faces.

How to Use
Step 1: Install Dependencies
Ensure Python is installed on your system.
Install required libraries:
bash
Copy code
pip install opencv-python face_recognition numpy

Step 2: Prepare Dataset
Add images of known individuals into a folder named Dataset/.
Each individual's images should be stored in a subfolder named after them. Example:
markdown
Copy code
Dataset/
├── student_1/
│   ├── image1.jpg
│   ├── image2.jpg
├── student_2/
    ├── image1.jpg
    ├── image2.jpg

Step 3: Run the Script
Execute the Python script:

bash
Copy code
python "Face Detection Based Attendance System.py"

Step 4: Quit and Save
The webcam will open, and the system will begin detecting and recognizing faces.
Press q to stop the program.
Check attendance_log.txt for the recorded attendance.
Requirements
Python 3.x
OpenCV
face_recognition
A working webcam
Future Enhancements
Add timestamps to the attendance log.
Improve the GUI for better usability.
Support for database integration to store attendance record 










