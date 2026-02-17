# 🧊 3D Reconstruction using Structure from Motion and NeRFs

## 📌 Overview

This project explores two fundamental approaches for **3D scene reconstruction from images**:

1. **Structure from Motion (SfM)** — reconstructing a 3D point cloud from real photographs.
2. **Neural Radiance Fields (NeRF)** — synthesizing novel views of a scene using deep learning.

The project was implemented using **OpenCV**, **PyTorch**, and Jupyter notebooks.

---

## 🎯 Project Objectives

The project was divided into two main parts:

### 🔹 Part 1 — Structure from Motion (SfM)

The goal was to reconstruct a **3D representation of a real-world object** using images captured with a smartphone.

Steps included:

- Capturing multiple images from different viewpoints
- Detecting keypoints using **SIFT**
- Matching features using **FLANN**
- Estimating camera poses
- Triangulating 3D points
- Generating a sparse point cloud reconstruction

The reconstructed object was a **laptop stand**, captured using an iPhone camera.

---

### 🔹 Part 2 — Neural Radiance Fields (NeRF)

The second part focused on **view synthesis using NeRFs**.

Due to time constraints, a reference implementation of **Tiny NeRF** was adapted and used to:

- Train a neural network on multi-view images
- Learn scene geometry and appearance
- Generate novel viewpoints via volumetric rendering

The NeRF model was trained on a standard dataset ("Lego truck scene").

---

## 🛠️ Technologies Used

- **Python**
- **OpenCV** — feature detection, matching, geometry
- **PyTorch** — neural network training
- **NumPy**
- **Matplotlib**
- **Jupyter / Google Colab**

---

## 📂 Repository Structure
.
├── StructureFromMotion.ipynb # SfM implementation notebook
├── NERF.ipynb # NeRF training and rendering notebook
├── report.pdf # Detailed project report
└── images/ # Example reconstruction results
---
## ▶️ How to Run

### Option 1 — Google Colab (Recommended)

Upload the notebooks to Google Colab and run all cells.

Both notebooks are self-contained and include:

- Data loading
- Processing pipeline
- Visualization steps

---

### Option 2 — Local Execution

Requirements:

```bash
pip install opencv-python torch numpy matplotlib
```
Then open:
```bash
StructureFromMotion.ipynb
NERF.ipynb
```
using Jupyter Notebook.

## 📊 Results
### SfM Reconstruction
* Successful sparse 3D point cloud reconstruction
* Accurate geometric structure from real smartphone images

### NeRF View Synthesis
* Learned volumetric scene representation
* Generated realistic novel viewpoints
* Demonstrated neural rendering pipeline

## 📚 Report
A detailed explanation of:
* Mathematical foundations
* Implementation details
* Challenges and limitations
* Experimental results

is available in:
report.pdf

## 🎓 Academic Context
This project was developed as part of a Computer Vision / 3D Reconstruction coursework, focusing on:
* Multi-view geometry
* Feature-based reconstruction
* Neural rendering techniques

## 👨‍💻 Author
Jorge Turriate
MSc in Mechatronics, Machine Vision & AI
Background in Computer Vision, Robotics, and Deep Learning

## 📄 License
For academic and educational purposes only.
