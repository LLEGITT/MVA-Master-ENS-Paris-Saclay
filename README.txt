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