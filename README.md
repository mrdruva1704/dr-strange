# dr-strange

This is a Python script that uses OpenCV and MediaPipe Hands to recognize hand gestures in real-time. The script captures video from the default camera and processes each frame to detect hand landmarks using MediaPipe Hands. Then, it calculates the distance between certain landmarks and draws lines between them according to the gesture recognized.

Installation
This script requires the following libraries to be installed:

cv2
mediapipe
To install the libraries, run the following command:

Copy code
pip install opencv-python mediapipe
Usage
Place the script and the "magic_circles" folder containing the magic circle images in the same directory.
Run the script using the following command:
Copy code
python hand_gesture_recognition.py
The script captures video from the default camera and detects hand gestures in real-time.
Features
This script recognizes two hand gestures:

Circle motion with two fingers

If the distance between the index finger and the little finger is 1.3 times greater than the distance between the wrist and the index finger, the script recognizes that the user is making a circular motion with their two fingers.
The script draws lines between the wrist and the tips of the thumb, index, middle, ring, and little fingers.
The script also draws lines between the tips of the thumb and the index, middle, ring, and little fingers.
Shield motion with five fingers

If the distance between the tips of the index finger and the little finger is between 0.5 and 1.3 times greater than the distance between the wrist and the index finger, the script recognizes that the user is making a shield motion with their five fingers.
The script draws a magic circle image on the middle point of the wrist and the index finger.
The script rotates the magic circle image in a counter-clockwise direction with an angular velocity of 2.0 degrees per frame.
License
This project is licensed under the MIT License - see the LICENSE file for details.





