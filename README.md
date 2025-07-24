🎥 Optical Flow Drawing Tool
This Python app lets you track a point in real-time using your webcam and draw its motion path using Lucas-Kanade Optical Flow. Think of it like a motion-controlled paintbrush where you guide the drawing with your hand or any moving object in the frame.

💡 Features
Live webcam feed

Select a point by clicking on the video

Tracks motion using OpenCV's Lucas-Kanade Optical Flow

Draws a tail/line representing the movement

Clear canvas with 'n' key

Exit anytime using the 'q' or Esc key

📦 Requirements
Install dependencies using pip:


Copy
Edit
pip install opencv-python numpy
🚀 How to Run
Just run the script:

Copy
Edit
python optical_flow_draw.py
Controls:
Left Click on the video to select a starting point to track

Press 'q' to stop tracking

Press 'n' to clear the path

Press Esc to exit

📸 Demo
Imagine waving your finger in front of the camera after selecting a point—it’ll trace a red line where the point moves!

🧠 How it Works
The webcam captures frames in real-time

User clicks a point on the frame to start tracking

The cv2.calcOpticalFlowPyrLK() function tracks the motion of that point across frames

As it moves, a red line is drawn from the previous to the current position

The mask stores this path and is overlaid on the video feed

🔧 File Breakdown
optical_flow_draw.py: Main Python script with OpenCV logic

🧼 Optional Enhancements
Track multiple points

Save the path as an image or video

Adjust color/thickness dynamically

Add smoothing or noise reduction

📃 License
This project is open-source. Feel free to use, modify, and share it.
