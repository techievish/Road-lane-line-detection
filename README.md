#Road Lane Line Detection


This project implements a road lane line detection system using computer vision techniques. The system processes video frames from a road video to identify and highlight lane lines.

Features
Perspective Transformation: Applies perspective transformation to get a bird's-eye view of the road.
Trackbars for Thresholding: Use trackbars to adjust the HSV thresholds for lane detection.

Object Detection: Detects lane lines using HSV color thresholding.

Histogram Analysis: Analyzes the histogram of the thresholded image to find lane line bases.
Sliding Window Technique: Uses sliding windows to detect lane lines along the road.

Polynomial Fitting: Fits second-order polynomials to the detected lane lines for smoother curvature.
Curvature Calculation: Calculates the curvature of the lane lines.

Lane Offset Calculation: Computes the offset of the vehicle from the center of the lane.

Steering Angle Calculation: Determines the steering angle required to stay in the lane.

Bird's Eye View Display: Displays a transformed bird's-eye view of the road with highlighted lane lines.

Original View Display: Overlays the detected lane lines on the original video frame.

Real-time Visualization: Provides real-time visualization of lane detection, curvature, offset, and steering angle.

Dependencies
OpenCV
NumPy

Installation
Clone the repository:git clone https://github.com/your-username/road-lane-line-detection.git
Install the required dependencies:pip install -r requirements.txt

Usage
Place your road video file in the project directory and name it road.mp4.
Run the road_lane_detection.py script:python road_lane_detection.py
Code Overview
Perspective Transformation: Chooses points for perspective transformation and applies the transformation to get a bird's-eye view of the road.

Trackbars for Thresholding: Creates trackbars for adjusting HSV thresholds.

Object Detection: Converts the transformed frame to HSV color space and applies thresholding to detect lane lines.

Histogram Analysis: Computes the histogram of the thresholded image to find the base positions of the lane lines.

Sliding Window Technique: Uses sliding windows to detect lane line pixels and fits second-order polynomials to the detected points.

Curvature Calculation: Calculates the curvature of the lane lines.

Lane Offset Calculation: Computes the offset of the vehicle from the center of the lane.

Steering Angle Calculation: Determines the steering angle based on the lane offset and curvature.

Visualization: Draws the detected lane lines and overlays them on the original and transformed frames. Displays the curvature, offset, and steering angle on the video frame.

License
This project is licensed under the MIT License
