# SnC

## Code Structure
This Python script utilizes the Intel RealSense depth camera through the pyrealsense2 and cv2 (OpenCV) libraries to display real-time depth information. The code structure is organized as follows:

Import necessary libraries (cv2 and pyrealsense2).

Import the DepthCamera class from the realsense_depth module.

Define a global variable point to represent a specific point on the screen.

Implement a mouse callback function show_distance to update the selected point when the mouse is clicked.

Initialize the RealSense depth camera using the DepthCamera class.

Create a window named "Color frame" and set up a mouse callback for user interaction.

Enter a loop to continuously capture depth and colour frames from the camera.

Display the depth frame with a highlighted circle at the selected point and show the corresponding depth value.

Exit the loop and close the windows when the 'Esc' key (key code 27) is pressed.

## Documentation
How to Use
1.	Ensure that the Intel RealSense depth camera (RGB-D sensor) and dobot magician are connected to your system.
2.	Install the required dependencies by running:
```bash
pip install opencv-python pyrealsense2
```
4.	Download the realsense_depth.py module place it in the same directory as the detect_depth.py file.
5.	Run the script by running:
```bash
Python detect_depth.py
```
7.	A window titled "Color frame" will appear, and you can click on any point to see the corresponding depth information in real-time.
8.	Press the 'Esc' key to exit the application.

## Functions
**show_distance(event, x, y, args, params)**

This function is a mouse callback that updates the global variable point with the coordinates of the mouse click.

## Dependencies
OpenCV (cv2): Used for image processing and displaying frames.

Intel RealSense SDK (pyrealsense2): Provides the interface for interacting with Intel RealSense depth cameras.

**Note:** The realsense_depth.py module is required for the code to work correctly. Please ensure it is downloaded and placed in the same directory as your script.

Download the code from pysource: https://pysource.com/2021/03/11/distance-detection-with-depth-camera-intel-realsense-d435i/
