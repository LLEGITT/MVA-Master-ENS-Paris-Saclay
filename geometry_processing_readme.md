# Geometry Processing and Geometric Deep Learning
**Master MVA (Mathématiques, Vision, Apprentissage) — ENS Paris-Saclay**

Ce dépôt contient le code, les travaux pratiques (TPs) et le projet de recherche pour le cours **Geometry Processing and Geometric Deep Learning**, enseigné dans le cadre du Master MVA à l'ENS Paris-Saclay (dispensé sur le site de l'Université Paris Cité).

---

## 🎯 Présentation du cours

Le cours **Geometry Processing and Geometric Deep Learning** explore les fondements mathématiques et informatiques permettant d'analyser, d'apprendre et de générer des données géométriques non-euclidiennes (nuages de points 3D, maillages/surfaces, variétés, champs d'orientations et représentations implicites).

### Enseignants :
* **Étienne Corman** (CNRS / LORIA)
* **Julie Digne** (CNRS / LIRIS, Université Claude Bernard Lyon 1)
* **Maks Ovsjanikov** (LIX, École Polytechnique)

---

## 📚 Programme & Sujets abordés

1. **Géométrie Différentielle Discrète & Opérateurs sur Surfaces :**
   * Opérateur de Laplace-Beltrami discrétisé via la méthode des éléments finis (FEM / Cotangent Weights).
   * Calcul de géodésiques (*Geodesics in Heat*) et signatures spectrales (HKS, WKS, GPS).
   * Paramétrisation de surfaces, déformation de formes, décomposition en recouvrements toriques et mise en correspondance (*Shape Matching*).

2. **Geometric Deep Learning & Représentations d'Apprentissage :**
   * Apprentissage sur maillages triangulaires et surfaces : convolutions intrinsèques (Geodesic CNNs), transport parallèle et traitement de features équivariantes par rotation.
   * Modèles multi-vues, volumétriques et sur nuages de points 3D : **PointNet**, **MeshCNN**, **DiffusionNet**, **DeltaConv**, **SpiralNet++**.
   * Champs de réseaux de neurones implicites (Neural Fields) et représentations continues : **DeepSDF**, **Occupancy Networks**, **SIREN**, **Implicit Displacement Fields** et réseaux de radiance (**NeRF**).
   * Modèles génératifs pour les formes 3D, espaces latents de formes et synthèse de nouvelles vues.

---

## 🛠️ Structure du dépôt & TPs

```text
├── tp1_differential_geometry/  # Opérateurs Laplaciens discrétisés, Équation de la chaleur & Géodésiques
├── tp2_surface_cnns/           # Convolutions intrinsèques sur surfaces & Features équivariantes par rotation
├── tp3_3d_deep_learning/       # PointNet, MeshCNN & Apprentissage intrinsèque
├── tp4_diffusionnet/           # DiffusionNet pour le traitement et la correspondance de maillages
├── tp5_neural_fields/          # Champs de distances signées implicites (DeepSDF, SIREN, IDF)
├── tp6_generative_models/      # Modèles génératifs de formes et Point2Mesh
├── project/                    # Projet final (Lecture, analyse critique et présentation d'article de recherche)
└── README.md
```

---

## 📊 Évaluation & Validation

* **Travaux Pratiques (10%) :** Évaluation des TPs (remise au fil des séances à l'adresse `GeometricDeepLearning@protonmail.com`).
* **Projet Final (90%) :** Présentation orale synthétique d'un article scientifique récent du domaine.
* **Mini-quiz :** Quiz d'auto-évaluation en début de séance pour valider l'assimilation des concepts.

---

## 🔗 Liens Utiles & Ressources

* **Page officielle du cours (MVA) :** [Geometry Processing and Geometric Deep Learning](https://www.master-mva.com/cours/geometry-processing-and-geometric-deep-learning/)
* **Site support du cours :** [mva_geom (Julie Digne)](https://jdigne.github.io/mva_geom/)
* **Site du Master MVA :** [master-mva.com](https://www.master-mva.com/)
* **ENS Paris-Saclay :** [ens-paris-saclay.fr](https://ens-paris-saclay.fr/)