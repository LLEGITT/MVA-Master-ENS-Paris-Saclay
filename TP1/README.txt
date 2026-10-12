# APM 53674 - ALTeGraD : Lab Session 1
## Neural Machine Translation and Language Modeling

Ce dépôt contient l'implémentation et le rapport du **Lab 1** du cours ALTeGraD (Prof. Michalis Vazirgiannis, TA: Yang Zhang & Amr Mohamed).

---

## 📌 Objectifs du Lab

L'objectif principal de ce TP est de construire et d'entraîner une architecture **Sequence-to-Sequence (Seq2Seq)** avec **Attention Globale** (type [Luong et al., 2015](https://arxiv.org/abs/1508.04025)) pour la traduction automatique de l'anglais vers le français.

### Concepts abordés :
- Implémentation sous **PyTorch** d'un Encodeur et d'un Décodeur à base de cellules **GRU** (Gated Recurrent Unit).
- Mécanisme d'**Attention Globale** (calcul de score par concaténation).
- Stratégie de décodage **Greedy Decoding**.
- Analyse des limites des modèles Seq2Seq classiques (hallucinations, sur-traduction, sous-traduction).
- Visualisation et interprétation des matrices d'alignement/attention.

---

## 🛠️ Structure du Notebook & Tâches

1. **Task 1 : Encoder** — Implémentation du passage avant (`forward`) de la classe `Encoder` (nn.Embedding + nn.GRU).
2. **Task 2 : Decoder** — Implémentation du décodeur pas à pas conditionné par le contexte source et le mot précédent.
3. **Task 3 : Attention Mechanism** — Implémentation du calcul des poids d'attention globales et du vecteur de contexte $c_t$.
4. **Task 4 : Seq2Seq Model** — Assemblage global de l'architecture (`seq2seqModel`) incluant la gestion du mode production (`predict`) et de la boucle d'entraînement (`fit`).
5. **Task 5 : Entraînement** — Vérification de la convergence de la perte sur le jeu de données Tatoeba.
6. **Task 6 : Inférence & Évaluation** — Évaluation du modèle pré-entraîné sur des phrases de test.

---

## ❓ Questions & Réponses théoriques

Le notebook contient les réponses détaillées aux questions suivantes :
* **Question 1 :** Analyse critique du *Greedy Decoding* vs *Beam Search*.
* **Question 2 :** Analyse des problèmes de sur-traduction et sous-traduction dans les modèles à attention basique.
* **Question 3 :** Code et matrice de heatmap pour visualiser les alignements attentionnels (inversion adjectif/nom en français/anglais).
* **Question 4 :** Gestion de la polysemie (ex: « *mean* ») et phénomènes d'hallucinations/boucles infinies.

---

## 📂 Données & Prérequis

- **Dataset :** ~136 521 paires d'entraînement / ~34 130 paires de test (Tatoeba / Anki).
- **Dépendances principales :**
  ```bash
  python >= 3.6
  torch
  nltk
  numpy
  matplotlib
  seaborn
  tqdm