# ARTI 403 — Lab 3: Image Manipulations using OpenCV

Student ID: 2440007196

## Contents

| File | Description |
|---|---|
| `Lab3_2440007196.ipynb` | Jupyter notebook with all code and outputs |
| `Lab3_Report_2440007196.pdf` | PDF report |
| `images/` | Input image and all output images |

## Tasks

| Task | Operation | Method |
|---|---|---|
| 1 | Enlarge | `cv2.resize`, scale 2x, cubic interpolation |
| 1 | Rotate 120° | `cv2.getRotationMatrix2D` + `cv2.warpAffine`, canvas enlarged to avoid cropping |
| 1 | Shear | affine matrix, factor 0.3 (horizontal and vertical) |
| 2 | Negative | `s = 255 - r` |
| 2 | Log | `s = c·log(1 + r)`, `c = 255 / log(256) = 45.99` |
| 2 | Power-law | `s = 255·(r/255)^γ`, `γ = 1.5` |

## Run

```
pip install opencv-python numpy matplotlib jupyter
jupyter notebook Lab3_2440007196.ipynb
```

Run all cells from top to bottom. Results are saved to `images/`.
