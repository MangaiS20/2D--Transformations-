# 2D--Transformations-
A Python toolkit for applying and visualizing 2D geometric transformations—featuring translation, rotation, scaling, shearing, reflection, affine, similarity, and projective techniques, all backed by mathematical foundations

 # 2D-Geometric-Transformations

This repository demonstrates the implementation of **2D Geometric Transformations** in Python using **NumPy** and **Matplotlib**.

The transformations covered include:

- **Translation** (shifting in x and y directions)
- **Rotation** (rotating about the origin)
- **Scaling** (uniform & non-uniform resizing)
- **Shearing** (slanting the shape)
- **Similarity Transformation** (rotation + translation + scaling)
- **Affine Transformation** (linear mapping + translation)
- **Projective Transformation (Homography)** (perspective distortion)

These are visualized on a **2D square** for clarity.

---

## 🔢 Mathematical Formulations

### 1. Homogeneous Coordinates
$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
=
T \cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

---

### 2. Translation
$$
T =
\begin{bmatrix}
1 & 0 & t_x \\
0 & 1 & t_y \\
0 & 0 & 1
\end{bmatrix}
$$

---

### 3. Rotation (angle $\theta$)
$$
R =
\begin{bmatrix}
\cos\theta & -\sin\theta & 0 \\
\sin\theta & \ \cos\theta & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

---

### 4. Scaling
$$
S =
\begin{bmatrix}
s_x & 0 & 0 \\
0 & s_y & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

---

### 5. Shearing
$$
Sh =
\begin{bmatrix}
1 & k_x & 0 \\
k_y & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

---

### 6. Similarity Transformation
Combination of scaling, rotation, and translation:
$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
=
\begin{bmatrix}
k\cos\theta & -k\sin\theta & t_x \\
k\sin\theta & \ \ k\cos\theta & t_y \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

---

### 7. Affine Transformation
$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
=
\begin{bmatrix}
a_{11} & a_{12} & t_x \\
a_{21} & a_{22} & t_y \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

---

### 8. Projective Transformation (Homography)
$$
\begin{bmatrix}
x' \\ y' \\ w
\end{bmatrix}
=
\begin{bmatrix}
h_{11} & h_{12} & h_{13} \\
h_{21} & h_{22} & h_{23} \\
h_{31} & h_{32} & h_{33}
\end{bmatrix}
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

After normalization:
$$
x' = \frac{x'}{w}, \qquad y' = \frac{y'}{w}
$$

---

## ⚡ Applications
- **Computer Vision** (image warping, registration)
- **Graphics** (object manipulation)
- **Robotics** (coordinate transformations)
- **Geometric Modeling**

---

## ▶️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/2D-Geometric-Transformations.git


## 🔹 Project Structure



📂 2D-Geometric-Transformations
┣ 📜 transformations.ipynb # Jupyter notebook with implementations
┣ 📜 README.md # Project documentation


---

## 🔹 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/2D-Geometric-Transformations.git
   cd 2D-Geometric-Transformations


Install dependencies:

pip install numpy matplotlib


Open the notebook:

jupyter notebook transformations.ipynb

📌 Applications

Image processing

Computer graphics

Computer vision (e.g., perspective correction)

Robotics & simulation
