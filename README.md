# 2D-Geometric-Transformations

This repository demonstrates the implementation of **2D Geometric Transformations** in Python using **NumPy** and **Matplotlib**.

The transformations covered include:

- **Translation** (shifting the object in x and y directions)
- **Rotation** (rotating about the origin)
- **Scaling** (uniform & non-uniform resizing)
- **Shearing** (slanting the shape)
- **Similarity Transformation** (rotation + translation + uniform scaling)
- **Affine Transformation** (linear mapping + translation)
- **Projective Transformation (Homography)** (general case with vanishing points & perspective distortion)

These transformations are visualized on a **2D square** for better understanding.

---

## 🔢 Mathematical Expressions

### 1. Homogeneous Coordinates Representation

![Homogeneous](https://latex.codecogs.com/png.latex?%5Cbegin%7Bbmatrix%7Dx%27%5C%5C%20y%27%5C%5C%201%5Cend%7Bbmatrix%7D%3D%20T%5Ccdot%5Cbegin%7Bbmatrix%7Dx%5C%5C%20y%5C%5C%201%5Cend%7Bbmatrix%7D)

---

### 2. Translation

![Translation](https://latex.codecogs.com/png.latex?T%3D%5Cbegin%7Bbmatrix%7D1%260%26t_x%5C%5C0%261%26t_y%5C%5C0%260%261%5Cend%7Bbmatrix%7D)

---

### 3. Rotation (angle θ)

![Rotation](https://latex.codecogs.com/png.latex?R%3D%5Cbegin%7Bbmatrix%7D%5Ccos%5Ctheta%20%26-%5Csin%5Ctheta%20%260%5C%5C%20%5Csin%5Ctheta%20%26%20%5Ccos%5Ctheta%20%260%5C%5C0%260%261%5Cend%7Bbmatrix%7D)

---

### 4. Scaling

![Scaling](https://latex.codecogs.com/png.latex?S%3D%5Cbegin%7Bbmatrix%7Ds_x%260%260%5C%5C0%26s_y%260%5C%5C0%260%261%5Cend%7Bbmatrix%7D)

---

### 5. Shearing

![Shearing](https://latex.codecogs.com/png.latex?Sh%3D%5Cbegin%7Bbmatrix%7D1%26k_x%260%5C%5Ck_y%261%260%5C%5C0%260%261%5Cend%7Bbmatrix%7D)

---

### 6. Similarity Transformation (rotation + scaling + translation)

![Similarity](https://latex.codecogs.com/png.latex?Sim%3D%5Cbegin%7Bbmatrix%7Dk%5Ccos%5Ctheta%20%26-k%5Csin%5Ctheta%20%26t_x%5C%5Ck%5Csin%5Ctheta%20%26k%5Ccos%5Ctheta%20%26t_y%5C%5C0%260%261%5Cend%7Bbmatrix%7D)

---

### 7. Affine Transformation

![Affine](https://latex.codecogs.com/png.latex?A%3D%5Cbegin%7Bbmatrix%7Da_%7B11%7D%26a_%7B12%7D%26t_x%5C%5Ca_%7B21%7D%26a_%7B22%7D%26t_y%5C%5C0%260%261%5Cend%7Bbmatrix%7D)

---

### 8. Projective Transformation (Homography)

![Projective](https://latex.codecogs.com/png.latex?H%3D%5Cbegin%7Bbmatrix%7Dh_%7B11%7D%26h_%7B12%7D%26h_%7B13%7D%5C%5Ch_%7B21%7D%26h_%7B22%7D%26h_%7B23%7D%5C%5Ch_%7B31%7D%26h_%7B32%7D%26h_%7B33%7D%5Cend%7Bbmatrix%7D)

![HomographyEq](https://latex.codecogs.com/png.latex?%5Cbegin%7Bbmatrix%7Dx%27%5C%5C%20y%27%5C%5C1%5Cend%7Bbmatrix%7D%20%5Csim%20H%5Ccdot%5Cbegin%7Bbmatrix%7Dx%5C%5C%20y%5C%5C%201%5Cend%7Bbmatrix%7D)

(where `~` means equality up to a scaling factor)

---

## ⚡ Applications
- **Computer Vision**
- **Image Processing**
- **Computer Graphics**
- **Geometric Modeling**

---

## ▶️ Usage

Clone this repo and run the notebook or Python scripts:

```bash
git clone https://github.com/yourusername/2D-Geometric-Transformations.git
cd 2D-Geometric-Transformations
python transformations.py
