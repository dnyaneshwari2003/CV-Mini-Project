
# 🧠 Computer Vision Mini Project: Feature Detection & Matching

## 📌 Project Overview

This project demonstrates how to **detect, describe, and match features** in images using well-known computer vision algorithms. The aim is to explore different techniques for keypoint detection and how they help in understanding and matching images, even under transformations like rotation, scale, or perspective changes.



## ✅ Tasks Covered

### 1. **SIFT (Scale-Invariant Feature Transform) Matching**

- **Objective**: Detect keypoints in two similar images and match them using SIFT.
- **Why SIFT?**  
  SIFT is robust to **scale, rotation, and illumination changes**. It's a popular algorithm used for tasks like image stitching, object recognition, and panorama creation.
- **Output**: A visualization of matched keypoints between two images and a stitched panoramic image using homography.

---

### 2. **Panorama Image Stitching with SIFT**

- **Objective**: Automatically stitch two overlapping images into one seamless panorama.
- **How?**  
  Keypoints are matched using SIFT, and a **homography transformation** is applied to warp and align one image with the other.
- **Output**: A single wide image combining the two input scenes.

---

### 3. **ORB (Oriented FAST and Rotated BRIEF)**

- **Why ORB instead of SURF?**  
  SURF is **patent-protected** and often not available in open environments like Google Colab. ORB is **free, fast, and efficient**, and works well for matching under **rotation and scale** changes.
- **Objective**: Detect and match keypoints between two images that differ in orientation and size.
- **Output**: Key point matches visualized between the two transformed images.

---

### 4. **Harris Corner Detection**

- **Objective**: Find corner points in an image — regions with strong intensity change in all directions.
- **Why Harris?**  
  It's a **classical method** useful for detecting **corners**, which are important for understanding shapes and features in an image.
- **Output**: The corners are marked clearly on the original image.

---

### 5. **Combined Feature Visualization (SIFT, ORB, Harris)**

- **Objective**: Compare the three detection methods side-by-side on the same image.
- **What it shows**:
  - **SIFT** gives robust and detailed keypoints.
  - **ORB** offers speed and scale/rotation invariance.
  - **Harris** highlights simple but effective corner detection.
- **Output**: A triptych visualization showing how each technique detects features differently.

---

## 🔧 Tools & Libraries Used

- `OpenCV`: For all computer vision operations including SIFT, ORB, and Harris.
- `NumPy`: For numerical operations and array manipulation.
- `Matplotlib`: For displaying images and visual results.

---

## 📁 Input Files

- Image pairs like `Taj1.jpeg`, `Taj2.jpeg`, `Taj_Mahal_scaled_rotated.png`, etc., used for testing feature detection and image stitching.

---

## 🎯 Learning Outcomes

- Understanding **keypoint detection** and **descriptor matching**.
- Applying **homography and warping** for image stitching.
- Comparing multiple feature detectors for robustness and efficiency.

