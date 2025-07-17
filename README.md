# Eye-Tracking-Mouse 

🎮 Eye Controlled Mouse: Hands-Free Cursor Control

🚀 Project Description

This Python script transforms your webcam into an innovative eye-controlled mouse, allowing you to move your cursor and perform clicks using only your head movements and blinks. Leveraging MediaPipe's advanced face mesh detection and PyAutoGUI, this project offers an alternative and accessible way to interact with your computer.

✨ Features

Real-time Face & Eye Tracking: Utilizes Google's MediaPipe Face Mesh to detect and track key facial landmarks, specifically focusing on eye movements.

Head-Controlled Cursor: Your head movements are mapped to your screen's cursor position, providing intuitive navigation.

Blink-to-Click Functionality: A detected blink (specifically, the closure of the left eye) triggers a mouse click, offering hands-free interaction.

Smoothed Cursor Movement: Implements a smoothing algorithm to reduce cursor jitter, providing a more fluid user experience.

Click Debouncing: Prevents multiple clicks from a single, prolonged blink, ensuring precise control.

Visual Feedback: Displays your webcam feed with real-time tracking points for debugging and user awareness.

Easy Exit: Press ESC at any time to close the application.

⚙️ Technologies Used

Python: The core programming language.

MediaPipe (Google): For robust and real-time facial landmark detection and tracking.

OpenCV (Open Source Computer Vision Library): For webcam access, frame processing, and displaying the visual output.

PyAutoGUI: For programmatic control of the mouse cursor and clicks on the operating system.

NumPy: Essential for numerical operations (implicitly used by MediaPipe/OpenCV).

💻 Setup and Installation

Prerequisites
Python 3.8 - 3.12 (64-bit recommended).

A webcam.

Installation Steps
Clone the Repository (or download the code):

git clone https://github.com/your-username/eye-controlled-mouse.git
cd eye-controlled-mouse
(Remember to replace your-username and eye-controlled-mouse.git with your actual GitHub repository URL once you upload it)

Create and Activate a Virtual Environment (Recommended):

python -m venv venv
On Windows (Command Prompt / PowerShell):

.\venv\Scripts\activate
On macOS / Linux (Bash / Zsh):

source venv/bin/activate
Install Required Libraries:
With your virtual environment activated, install the necessary libraries:

pip install mediapipe opencv-python pyautogui

🚀 How to Use

Run the Script:
Ensure your virtual environment is activated, then run the script from your project directory:

python your_script_name.py
(Replace your_script_name.py with the actual filename of your Python script, e.g., eye_mouse.py)

Control the Mouse:

Position your face clearly in front of the webcam.

Move your head to guide the mouse cursor around your screen.

Perform a blink to register a mouse click.

You might need to adjust the SMOOTHING_FACTOR and CLICK_THRESHOLD values in the code for optimal performance based on your webcam and lighting conditions.

Exit the Application:

Press the ESC key on your keyboard at any time to close the application window.

📝 Notes

Ensure your room is well-lit for optimal face and eye detection.

The system primarily maps head movement to cursor movement. For true "gaze" tracking, more advanced algorithms would be required.

If the webcam doesn't open, check your system's privacy settings to ensure applications have access to your camera.

💡 Future Enhancements (Ideas for Contribution!)

Calibration UI: Add a simple user interface for calibrating blink sensitivity and mouse speed.

Different Click Types: Implement double-click, right-click, or drag-and-drop based on different gestures (e.g., specific blinks, sustained eye closure).

Gaze Tracking: Implement more sophisticated gaze estimation for true eye-controlled movement.

Accessibility Features: Integrate scrolling (e.g., based on vertical head tilt) or zoom.

Head Pose Correction: Compensate for slight head rotations for more stable cursor control.

User Profiles: Save and load calibration settings for different users or environments.
