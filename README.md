
# 📌 2D-Geometric-Transformations  

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

![Homogeneous](https://latex.codecogs.com/png.latex?\begin{bmatrix}x'\\y'\\1\end{bmatrix}=T\cdot\begin{bmatrix}x\\y\\1\end{bmatrix})  

---

### 2. Translation  

![Translation](https://latex.codecogs.com/png.latex?\begin{bmatrix}1&0&t_x\\0&1&t_y\\0&0&1\end{bmatrix})  

---

### 3. Rotation (angle θ)  

![Rotation](https://latex.codecogs.com/png.latex?\begin{bmatrix}\cos\theta&-\sin\theta&0\\\sin\theta&\cos\theta&0\\0&0&1\end{bmatrix})  

---

### 4. Scaling  

![Scaling](https://latex.codecogs.com/png.latex?\begin{bmatrix}s_x&0&0\\0&s_y&0\\0&0&1\end{bmatrix})  

---

### 5. Shearing  

![Shearing](https://latex.codecogs.com/png.latex?\begin{bmatrix}1&k_x&0\\k_y&1&0\\0&0&1\end{bmatrix})  

---

### 6. Similarity Transformation (rotation + scaling + translation)  

![Similarity](https://latex.codecogs.com/png.latex?\begin{bmatrix}k\cos\theta&-k\sin\theta&t_x\\k\sin\theta&k\cos\theta&t_y\\0&0&1\end{bmatrix})  

---

### 7. Affine Transformation  

![Affine](https://latex.codecogs.com/png.latex?\begin{bmatrix}a_{11}&a_{12}&t_x\\a_{21}&a_{22}&t_y\\0&0&1\end{bmatrix})  

---

### 8. Projective Transformation (Homography)  

![Projective](https://latex.codecogs.com/png.latex?\begin{bmatrix}h_{11}&h_{12}&h_{13}\\h_{21}&h_{22}&h_{23}\\h_{31}&h_{32}&h_{33}\end{bmatrix})  

And the mapping:  

![Homography Mapping](https://latex.codecogs.com/png.latex?\begin{bmatrix}x'\\y'\\1\end{bmatrix}\sim H\cdot\begin{bmatrix}x\\y\\1\end{bmatrix})  

(where `~` means equality up to a scaling factor).  

---

⚡This repo is useful for **Computer Vision**, **Image Processing**, and **Graphics students** to understand how transformations work both mathematically and visually.  
