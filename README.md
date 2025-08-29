# 2D--Transformations-
A Python toolkit for applying and visualizing 2D geometric transformations—featuring translation, rotation, scaling, shearing, reflection, affine, similarity, and projective techniques, all backed by mathematical foundations

# 2D Geometric Transformations



This project demonstrates *2D geometric transformations* in Python, including:



- *Translation*

- *Scaling*

- *Rotation*

- *Reflection*

- *Shear*

- *Similarity Transformation*

- *Affine Transformation*

- *Projective Transformation*



The transformations are implemented using *NumPy* and *Matplotlib* for visualization, making it easy to understand how each transformation modifies a given shape.



---



## 🔹 Mathematical Background



### 1. Translation

$$

\begin{bmatrix}

x' \\ y' \\ 1

\end{bmatrix}

=

\begin{bmatrix}

1 & 0 & t_x \\

0 & 1 & t_y \\

0 & 0 & 1

\end{bmatrix}

\cdot

\begin{bmatrix}

x \\ y \\ 1

\end{bmatrix}

$$



### 2. Scaling

$$

\begin{bmatrix}

x' \\ y' \\ 1

\end{bmatrix}

=

\begin{bmatrix}

s_x & 0 & 0 \\

0 & s_y & 0 \\

0 & 0 & 1

\end{bmatrix}

\cdot

\begin{bmatrix}

x \\ y \\ 1

\end{bmatrix}

$$



### 3. Rotation

$$

\begin{bmatrix}

x' \\ y' \\ 1

\end{bmatrix}

=

\begin{bmatrix}

\cos\theta & \sin\theta & 0 \\

-\sin\theta & \cos\theta & 0 \\

0 & 0 & 1

\end{bmatrix}

\cdot

\begin{bmatrix}

x \\ y \\ 1

\end{bmatrix}

$$



### 4. Reflection

Reflection across the x-axis:

$$

\begin{bmatrix}

x' \\ y' \\ 1

\end{bmatrix}

=

\begin{bmatrix}

1 & 0 & 0 \\

0 & -1 & 0 \\

0 & 0 & 1

\end{bmatrix}

\cdot

\begin{bmatrix}

x \\ y \\ 1

\end{bmatrix}

$$



### 5. Shear

$$

\begin{bmatrix}

x' \\ y' \\ 1

\end{bmatrix}

=

\begin{bmatrix}

1 & k_x & 0 \\

k_y & 1 & 0 \\

0 & 0 & 1

\end{bmatrix}

\cdot

\begin{bmatrix}

x \\ y \\ 1

\end{bmatrix}

$$



### 6. Similarity Transformation

Combination of scaling, rotation, and translation:

$$

\begin{bmatrix}

x' \\ y' \\ 1

\end{bmatrix}

=

\begin{bmatrix}

s\cos\theta & s\sin\theta & t_x \\

-s\sin\theta & s\cos\theta & t_y \\

0 & 0 & 1

\end{bmatrix}

\cdot

\begin{bmatrix}

x \\ y \\ 1

\end{bmatrix}

$$



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

\cdot

\begin{bmatrix}

x \\ y \\ 1

\end{bmatrix}

$$



### 8. Projective Transformation

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

\cdot

\begin{bmatrix}

x \\ y \\ 1

\end{bmatrix}

$$



Final coordinates after normalization:

$$

x' = \frac{x'}{w}, \quad y' = \frac{y'}{w}

$$



---



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
