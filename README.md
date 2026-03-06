# Image Processing using OpenCV (Python)

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)<br>
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green)<br>
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)<br>
![Status](https://img.shields.io/badge/Project-Completed-success)<br>

A beginner-friendly **Computer Vision project** demonstrating fundamental **Image Processing techniques using OpenCV in Python**.<br>

This project helps understand how digital images are processed using operations like **grayscale conversion, thresholding, edge detection, and webcam capture**.<br>

---

# Project Preview

The notebook demonstrates:<br>

- Image loading and visualization<br>
- Image matrix representation<br>
- Color space conversion<br>
- Image preprocessing<br>
- Edge detection<br>
- Real-time webcam capture<br>

---

# Technologies Used

| Technology | Purpose |<br>
|-------------|--------|<br>
| Python | Programming language |<br>
| OpenCV | Image Processing |<br>
| Matplotlib | Image Visualization |<br>
| Jupyter Notebook | Development environment |<br>

---

# Project Structure

Image-Processing-OpenCV/<br>

│

├── 01_Image_Processing.ipynb<br>
├── README.md<br>
│<br>
└── images<br>
├── Lemon.jpg<br>
├── Mango1.jpg<br>
└── Rose.jpg<br>


---

# Features Implemented

### 1 Image Loading

``python
img = cv2.imread("Lemon.jpg")
Loads image from system using OpenCV.``

### 2 Image Information
``
print(img.shape)
(height, width, channels) ``

### 3 3 BGR → RGB Conversion
``img_rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)``

### 4 Grayscale Conversion
``gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
Used for preprocessing before edge detection or thresholding.``

### 5 Thresholding
``_, thresh = cv2.threshold(gray, 127, 255, cv2.THRESH_BINARY)
Converts image into binary format.``

### 6 Edge Detection (Canny)
``edges = cv2.Canny(gray,100,200)
Detects object boundaries in images.``

### 7 Sobel Edge Detection
``Used to detect horizontal and vertical edges.
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0)
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1)``

### 8 Webcam Capture
``cap = cv2.VideoCapture(0)
Captures frames from the system webcam for real-time processing.``

## Installation

**Install required libraries:**<br>
`pip install opencv-python matplotlib`<br>
*Or using Anaconda*<br>
*conda install opencv matplotlib*<br>

## How to Run
*Step 1*<br>
Clone the repository<br>
git clone `https://github.com/yourusername/image-processing-opencv.git`<br>

*Step 2*
Navigate to folder<br>
cd image-processing-opencv<br>

*Step 3*
Start Jupyter Notebook<br>
jupyter notebook<br>

*Step 4*
Open<br>
01\_Image\_Processing.ipynb<br>
Run cells sequentially.<br>

## Important Note (Google Colab Users)
*Some cells use*<br>
`cv2.imshow()`<br>
⚠ This function does NOT work in Google Colab because Colab does not support GUI windows.<br>

Example:<br>
cv2.imshow("Camera Test", frame)<br>

**This works only in:**
- Jupyter Notebook (Local)<br>
- Anaconda<br>
- VS Code Python<br>
- Spyder IDE<br>

**Alternative for Google Colab:**<br>
Use Matplotlib display instead<br>
import matplotlib.pyplot as plt<br>
`plt.imshow(frame)<br>
plt.axis("off")`<br>

## Learning Outcomes
**After completing this project you will understand:**<br>
- Image matrix representation<br>
- Color space conversion<br>
- Image preprocessing<br>
- Thresholding<br>
- Edge detection techniques<br>
- Real-time image processing<br>

## Future Improvements
**Possible extensions:**<br>
- Face Detection<br>
- Object Detection<br>
- Image Segmentation<br>
- Deep Learning based Computer Vision<br>
- Real-time video analytics<br>

## Author
**Abbu Talib Ansari**<br>
`GitHub:https//github.com/talibansari1914`
