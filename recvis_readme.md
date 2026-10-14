# Object Recognition and Computer Vision (RecVis)

**Master MVA (Mathematics, Vision, Learning) — ENS Paris-Saclay**

This repository contains the code, assignments, and research project for the **Object Recognition and Computer Vision** (RecVis / Reconnaissance d'Objets et Vision Artificielle) course, taught as part of the M2 MVA Master's program at **ENS Paris-Saclay**.

## 🎯 Course Overview

Automatic object recognition—and more generally, understanding scenes from photographs and video—is one of the primary challenges in **Computer Vision**. This course explores classical and modern models of images, objects, and scenes, as well as foundational and contemporary algorithms (handcrafted representations, deep neural networks, self-supervised learning, and vision-language models) used to tackle these tasks.

### Instructors & Lecturers:

* **Jean Ponce** (INRIA / ENS Ulm / NYU)
* **Cordelia Schmid** (INRIA / Google Research)
* **Ivan Laptev** (INRIA / MBZUAI)
* **Mathieu Aubry** (École des Ponts ParisTech / LIGM)
* **Gül Varol** (École des Ponts ParisTech / LIGM)

---

## 📚 Curriculum & Topics Covered

1. **Foundations of Classical Computer Vision:**
   * Local feature extraction and invariance (SIFT, HOG, RANSAC).
   * Image matching, multi-view geometry, and keypoint correspondence.
   * Bag of Visual Words (BoVW), Deformable Part Models (DPM).

2. **Deep Learning for Object Recognition:**
   * Convolutional networks (CNNs), modern backbones (ResNet, ConvNeXt), and Vision Transformers (ViT).
   * Image classification, backpropagation, optimization, and regularization.
   * Object Detection: two-stage frameworks (Faster R-CNN) and end-to-end transformers (YOLO, DETR).
   * Image Segmentation: Semantic (FCN, Mask2Former) and Instance/Panoptic Segmentation (Mask R-CNN).

3. **Modern Representation Learning & Foundational Models:**
   * Self-Supervised Learning (SSL): contrastive frameworks (SimCLR, MoCo) and Masked Image Modeling (MAE).
   * Vision-Language representations and Foundation Models (CLIP, ALIGN, LLaVA).
   * Action recognition and spatio-temporal 3D video understanding.

---

## 🛠️ Repository Structure

```text
├── assignment1_cnn_classification/   # Image classification with CNNs, PyTorch, and transfer learning
├── assignment2_object_detection/     # Object detection and segmentation (Faster R-CNN, Mask R-CNN, DETR)
├── assignment3_self_supervised/      # Visual representation learning (SimCLR, MAE, CLIP)
├── final_project/                    # Research project (code, report, and presentation slides)
└── README.md
```

---

## 📊 Evaluation & Grading Scheme

* **Programming Assignments (50%):**
  * **Assignment 1 (10%):** Image classification and convolutional neural network architectures.
  * **Assignment 2 (20%):** Object detection and semantic/instance segmentation.
  * **Assignment 3 (20%):** Self-supervised visual representation learning & vision-language models.
* **Final Research Project (50%):** An individual or paired research project addressing an open computer vision problem (written report in CVPR/ICCV conference format + oral defense).

---

## 🔗 Useful Links & Resources

* **Official Course Webpage (RecVis):** [RecVis Course Webpage](https://gulvarol.github.io/teaching/recvis24/)
* **Master MVA Website:** [master-mva.com](https://www.master-mva.com/)
* **INRIA Willow Research Group:** [Willow Group](https://www.di.ens.fr/willow/)
* **ENS Paris-Saclay:** [ens-paris-saclay.fr](https://ens-paris-saclay.fr/)