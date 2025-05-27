# Corner_Detector
arris Corner Detection with Multi-Scale Analysis
#📝 Overview
This project implements Harris Corner Detection using OpenCV, and explores the effect of window size and image scaling on corner detection accuracy.

It is divided into two main tasks:

#📌 Task 1: Fixed Image Scale, Varying Window Size
A grayscale image is passed to the Harris Corner Detector.

The window size (kernel size) is varied using powers of 2 (e.g., 2, 4, 8, ..., 64).

The number of detected corners is counted and compared to a known correct value (e.g., 78 or 80).

If the number of detected corners matches the expected count, the result is displayed with annotations.

#🔍 Purpose:
To analyze how changing the Harris window size affects corner detection at a fixed scale.

#📌 Task 2: Image Pyramids (Scaling Down), Varying Window Size
The image is gradually scaled down using pyramid downsampling (cv2.pyrDown).

For each scale, the Harris Corner Detector is applied with varying window sizes.

This simulates detecting corners at multiple resolutions, mimicking real-world scenarios where objects appear at different scales.

#🔍 Purpose:
To examine whether the Harris Corner Detector maintains accuracy and consistency across image scales, and how window size interacts with image resolution.
