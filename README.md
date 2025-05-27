# Corner_Detector

# 🟩 Harris Corner Detection with Multi-Scale Pyramids

This project implements Harris Corner Detection using OpenCV and explores how corner detection behaves under different scales and window sizes. The project is divided into two main tasks:

---

## 📌 Task Breakdown

### ✅ Task 1: Varying Window Sizes
Detect corners on the **original image** using different window sizes for the Harris corner detector.

- Uses OpenCV’s `cv2.cornerHarris`.
- Iterates over multiple window sizes (`2^k` where `k` from 1 to 6).
- Highlights corners in green if the number of detected corners matches a known count (e.g., 78 or 80).
- Displays result with `cv2.putText` showing window size and corner count.

### ✅ Task 2: Image Pyramid Scaling
Detect corners while **scaling down the image**, mimicking how the corner detector behaves in a pyramid-like approach.

- Each scale level downsamples the image (e.g., scale 0, 1, 2).
- Window size remains constant, but image resolution changes.
- Helps evaluate the stability of corner detection across scales.

---

## 🧪 Input

Two images used for comparison:

- `1.PNG`: First logo/image
- `3.PNG`: Second logo/image

You can replace them with your own for testing.

---

## 🖥️ Output

- Visual display of corners for each configuration.
- Text overlay with detected window size and number of corners.
- Comparison of image sizes to determine which logo is smaller/larger based on pixel area.



