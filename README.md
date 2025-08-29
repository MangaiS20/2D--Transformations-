# 2D--Transformations-
A Python toolkit for applying and visualizing 2D geometric transformations—featuring translation, rotation, scaling, shearing, reflection, affine, similarity, and projective techniques, all backed by mathematical foundations

 *Description* you can use for your GitHub repository 👇

---

### 📌 Repository Name:

2D-Geometric-Transformations

---

### 📝 Description (for README):

This repository demonstrates the implementation of *2D Geometric Transformations* in Python using *NumPy* and *Matplotlib*.

The transformations covered include:

* *Translation* (shifting the object in x and y directions)
* *Rotation* (rotating about the origin)
* *Scaling* (uniform & non-uniform resizing)
* *Shearing* (slanting the shape)
* *Similarity Transformation* (rotation + translation + uniform scaling)
* *Affine Transformation* (linear mapping + translation)
* *Projective Transformation (Homography)* (general case with vanishing points & perspective distortion)

These transformations are visualized on a *2D square* for better understanding.

---

### 🔢 Mathematical Expressions

1. *Homogeneous Coordinates Representation*

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

where $T$ is the transformation matrix.

---


2. *Translation*

$$
T = 
\begin{bmatrix}
1 & 0 & t_x \\
0 & 1 & t_y \\
0 & 0 & 1
\end{bmatrix}
$$

---

3. *Rotation* (angle $\theta$)

$$
R = 
\begin{bmatrix}
\cos\theta & -\sin\theta & 0 \\
\sin\theta & \cos\theta & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

---

4. *Scaling*

$$
S = 
\begin{bmatrix}
s_x & 0 & 0 \\
0 & s_y & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

---

5. *Shearing*

$$
Sh = 
\begin{bmatrix}
1 & k_x & 0 \\
k_y & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

---

6. *Similarity Transformation* (rotation + scaling + translation)

$$
Sim = 
\begin{bmatrix}
k\cos\theta & -k\sin\theta & t_x \\
k\sin\theta & k\cos\theta & t_y \\
0 & 0 & 1
\end{bmatrix}
$$

---

7. *Affine Transformation*

$$
A = 
\begin{bmatrix}
a_{11} & a_{12} & t_x \\
a_{21} & a_{22} & t_y \\
0 & 0 & 1
\end{bmatrix}
$$

---

8. *Projective Transformation (Homography)*

$$
H = 
\begin{bmatrix}
h_{11} & h_{12} & h_{13} \\
h_{21} & h_{22} & h_{23} \\
h_{31} & h_{32} & h_{33}
\end{bmatrix}
$$

$$
\begin{bmatrix}
x' \\ y' \\ 1
\end{bmatrix}
\sim
H \cdot
\begin{bmatrix}
x \\ y \\ 1
\end{bmatrix}
$$

(where $\sim$ means equality up to a scaling factor).

---

⚡This repo is useful for *Computer Vision, **Image Processing, and **Graphics students* to understand how transformations work both mathematically and visually.

---


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
