Here are the two `README.txt` files for the Geometry Deep Learning practical sessions, written in English:

---

### README for Lab 1 (Laplace-Beltrami, Diffusion, and HKS)

```text
# MVA / GDL : Practical Session 1
## Laplace-Beltrami Operator, Surface Diffusion, and HKS

This repository contains the implementation and report for **Lab 1** of the Geometry Deep Learning course.

---

## 📌 Lab Objectives

The main objective of this lab is to explore the use of the Laplacian operator on a triangulated surface (mesh) to solve heat diffusion, perform shape matching, and compute spectral signatures.

### Concepts Covered:
- Reading and storing triangulated surfaces in `.off` format.
- Constructing the discrete Laplace-Beltrami operator (mass matrix $A$ and stiffness matrix $W$).
- Simulating exact heat diffusion (via sparse linear systems) and spectral diffusion (via eigen-decomposition).
- Computing the Heat Kernel Signature (HKS) as an isometry-invariant descriptor.
- (Bonus) Implementing the heat method for geodesic distance computation.

---

## 🛠️ Notebook Structure & Tasks

1. **Task 1: Mesh Loading** — Implementation of the `read_off` function and the `MyMesh` class to handle vertices and faces.
2. **Task 2: Discrete Operators (Areas)** — Computing face areas and the diagonal mass matrix $A$.
3. **Task 3: Cotangent Matrix** — Computing cotangent weights and the stiffness matrix $W$.
4. **Task 4: Exact Diffusion** — Solving the sparse linear system to simulate heat diffusion over time.
5. **Task 5 & 6: Spectral Decomposition & HKS** — Computing Laplacian eigenvalues/eigenvectors and generating the HKS descriptor.
6. **Task 7: Heat Method (Bonus)** — Using gradient and divergence operators to estimate geodesics.

---

## ❓ Questions & Theoretical Answers

The notebook contains detailed answers to the following questions:
* **Questions 1 to 3:** Verifying area consistency and the zero-sum property of the cotangent matrix rows.
* **Questions 4 & 5:** Analyzing the diffusion of a Dirac-like function on a mesh over time $t$.
* **Questions 6 to 8:** Comparing exact diffusion and the spectral approach depending on the size of the eigenbasis.
* **Questions 9 & 10:** Using HKS to establish shape correspondences between different surfaces.

---

## 📂 Data & Prerequisites

- **Dataset:** 3D meshes (e.g., `bunny.off`, `hand1`, `hand2`).
- **Main Dependencies:**
  ```bash
  numpy
  scipy
  matplotlib
  meshplot

```

```

---

### README for Lab 2 (Surface Parameterization and Deformation)

```text
# MVA / GDL : Practical Session 2
## Surface Parameterization and Deformation

This repository contains the implementation and report for **Lab 2** of the Geometry Deep Learning course.

---

## 📌 Lab Objectives

The main objective of this lab is to explore surface deformation and alignment algorithms through two major applications: surface parameterization for texture mapping and non-rigid shape alignment.

### Concepts Covered:
- Extracting and managing border edges.
- Generating equidistant points on a circle for boundary conditions.
- Tutte embedding via constrained linear system solving.
- Rigid alignment using ICP (Iterative Closest Point).
- Non-rigid deformation using ARAP (As-Rigid-As-Possible).

---

## 🛠️ Notebook Structure & Tasks

1. **Task 1: Border Edges** — Implementing the `get_border_edges` function to identify surface boundaries.
2. **Task 2: Points on a Circle** — Writing a function to generate uniformly distributed points on a unit circle.
3. **Task 3: Tutte Embedding** — Solving the sparse linear system to assign planar coordinates $(u, v)$ to internal vertices while fixing boundaries.
4. **Task 4: Rigid Alignment (ICP)** — Setting up the Iterative Closest Point algorithm.
5. **Task 5: ARAP Deformation** — Implementing the As-Rigid-As-Possible approach for non-rigid surface alignment.

---

## ❓ Questions & Theoretical Answers

The notebook contains detailed answers to the following questions:
* **Question 1:** Identifying and validating the topological border edges of a cut mesh.
* **Questions 2 & 3:** Analyzing Tutte parameterization and visualizing texture mapping on an open sphere.
* **Questions 4 & 5:** Evaluating geometric alignment performance between rigid and non-rigid shapes.

---

## 📂 Data & Prerequisites

- **Dataset:** 3D objects and textures (e.g., `sphere_cut_uv.obj`).
- **Main Dependencies:**
  ```bash
  numpy
  scipy
  matplotlib
  meshplot
  mesh_utils

```

```

```