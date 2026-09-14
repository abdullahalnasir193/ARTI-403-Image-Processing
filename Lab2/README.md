# ARTI 403 – Lab 2: Image Sampling, Quantization & Arithmetic/Set Operations

## Overview
Solution for Lab 2 (Digital Image Fundamentals). Covers image sampling, quantization, arithmetic operations, and set/logical operations on grayscale images.

## Requirements
- Python 3
- OpenCV (`opencv-python`)
- Pillow
- NumPy
- Matplotlib

Install:
```bash
pip install opencv-python pillow numpy matplotlib
```

## Folder Structure
```
repo/
├── images/
│   ├── lena_gray_256.tif
│   ├── cameraman.tif
│   ├── A.png
│   └── B.png
└── lab2/
    ├── lab2_solution.ipynb
    └── README.md
```

## Tasks

**Task 1 — Sampling & Quantization**
Downsamples and quantizes `lena_gray_256.tif` at multiple parameter combinations (factor/levels: 2/2, 4/4, 14/9) to show the effect of each parameter.

**Task 2 — Arithmetic & Set Operations**
Loads `lena_gray_256.tif`, `cameraman.tif`, `A.png`, `B.png` (resized to 400×400) and computes:
- Subtraction of two grayscale images
- Addition of a constant value (175) to an image
- Set difference (A − B)
- Symmetric difference (A XOR B)
- Intersection (A AND B)

## How to Run
1. Place the four required images inside `../images/` relative to the notebook.
2. Open `lab2_solution.ipynb` in Jupyter.
3. Run all cells top to bottom.
