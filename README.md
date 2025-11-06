📖 Project Overview

This project turns your webcam into a motion detector using Python and OpenCV.
It continuously monitors the camera feed, detects any movement, highlights it with a rectangle, and plays a beep sound whenever motion is detected — just like a basic security camera alert system.

⚙️ Features

📸 Captures live video from your webcam

🎯 Detects movement in real time

🔔 Plays an alert beep when motion is detected

🟩 Highlights the moving area with a green rectangle

⏹️ Easily stop the system by pressing the ESC key

🧰 Technologies Used

Python 3

OpenCV (cv2) – for image processing and motion detection

Winsound – for beep alert sound (Windows only)

🚀 How It Works

The webcam captures two consecutive frames (images).

The program compares them to detect any difference (motion).

The areas with motion are highlighted and a beep sound is played.

The live camera feed with highlighted motion is shown on the screen.

Press the ESC key to stop the program.

💻 Setup Instructions

Install Dependencies

pip install opencv-python


(No need to install winsound — it comes with Python on Windows)

Run the Script

python security_camera.py


Allow Camera Access

Make sure your webcam is connected and allowed for use.

📜 Code Explanation (in short)
Step	Description
1	Open webcam and capture video frames
2	Compare two frames to find movement
3	Convert image to grayscale for processing
4	Highlight movement areas using threshold
5	Find and mark moving objects with rectangles
6	Play beep sound to alert user
7	Display live video feed and press ESC to exit
⚠️ Notes

The beep alert (winsound.Beep) works only on Windows.

You can adjust the motion sensitivity by changing this value:

if area < 5000:
    continue


→ Lower it for smaller motion detection, raise it for larger motion only.

✨ Example Use Cases

Home security motion detector

Office activity monitor

Simple project to learn OpenCV basics

🧑‍💻 Author

Sarthak Dua
💡 Passionate about Data & AI projects | Exploring Python, Computer Vision, and Analytics
