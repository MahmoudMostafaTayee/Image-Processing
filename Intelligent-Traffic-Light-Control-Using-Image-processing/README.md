# Intelligent Traffic Light Control Using Image Processing

🚦 A computer vision-based system for detecting and tracking cars in traffic footage, intended for real-time intelligent traffic light control.

## Overview

This project utilizes **image processing** and **real-time object tracking** to monitor traffic density by detecting and tracking moving cars across video frames. Based on the analysis, such a system could be extended to dynamically control traffic lights, giving priority to congested directions.

---

## Features

- 🚘 **Car Detection** using frame differencing and contour extraction
- 🎯 **Real-Time Object Tracking** with ID assignment
- 📹 **Video Output** showing detected cars with bounding boxes and labels
- 🧠 Framework for **intelligent traffic light** logic (to be integrated)

---

## Technologies Used

- Python
- OpenCV (cv2)
- NumPy
- Basic image differencing & morphological operations
- Custom tracking logic based on Euclidean distance


---

## How It Works

1. **Load Frames:** Reads consecutive frames from a video source.
2. **Preprocessing:** Converts frames to grayscale and applies absolute difference.
3. **Motion Detection:** Applies binary thresholding and dilation to highlight moving objects (cars).
4. **Contour Extraction:** Identifies car-like contours in a region of interest (ROI).
5. **Tracking:** Uses a custom class to assign consistent IDs to detected cars based on distance.
6. **Visualization:** Annotates the original video frames with bounding boxes and IDs.
7. **Output:** Saves the annotated video with tracked car movements.


